# Twig-Extension-Number

[![Travis Build Status](https://travis-ci.org/thePanz/Twig-Extension-Number.svg?branch=1.x)](https://travis-ci.org/thePanz/Twig-Extension-Number) [![Latest Stable Version](https://poser.pugx.org/pnz/twig-extension-number/v/stable.svg)](https://packagist.org/packages/pnz/twig-extension-number) [![Total Downloads](https://poser.pugx.org/pnz/twig-extension-number/downloads.svg)](https://packagist.org/packages/pnz/twig-extension-number) [![Latest Unstable Version](https://poser.pugx.org/pnz/twig-extension-number/v/unstable.svg)](https://packagist.org/packages/pnz/twig-extension-number) [![License](https://poser.pugx.org/pnz/twig-extension-number/license.svg)](https://packagist.org/packages/pnz/twig-extension-number) [![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/thePanz/Twig-Extension-Number/badges/quality-score.png?b=1.x)](https://scrutinizer-ci.com/g/thePanz/Twig-Extension-Number/?branch=1.x)


A Twig extension to handle number formatting.

Included filters:

 - `format_bytes` : Format the given amount as bytes and display it in an as a human readable format.
   The filter supports 1000/1024 base counting and formatting
   
 - `format_grams` : Format the given amount as "grams" in an human readable format
 
 - `format_meters` : Format the given amount as "meters" in an human readable format


## Examples

Display the value 4000 grams in a human readable format (4.00 Kg):
```
{{ 4000 | format_grams }}
```

[Decimals] Display the value 4000 grams in a human readable format with 3 decimals (4.000 Kg):
```
{{ 4000 | format_grams(3) }}
```

[UnityBias] Display the value 4000 milligrams as grams in a human readable format with 3 decimals (4.00 g):
```
{{ 4000 | format_grams(3, 1E-3) }}
```


## Todo
 - [] Implement I18n of number values
 - [] Implement `format_liters` filter
