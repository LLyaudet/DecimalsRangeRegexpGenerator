# DecimalsRangeRegexpGenerator
Handle min, max and step to produce a regular expression for ranges of decimal numbers.

Several integers range regular expression generators can be found on github,
but they do not handle decimal numbers.
(Decimal numbers are the subset of the rational numbers that can be written
as n/10^k where n and k are integers.)
They can handle min and max parameters, but they do not handle step parameter.

The goal of this dev tool is to have an easy path to avoid most use cases of HTML's:

    <input type="number" min="@some_decimal1@" max="@some_decimal2@" step="@some_decimal3@">

by using

    <input type="text" inputmode="numeric" pattern="@some_regexp@">

instead.

For a few reasons to replace input number with input text and a pattern,
you may read the following blog articles or webpages:
- https://technology.blog.gov.uk/2020/02/24/why-the-gov-uk-design-system-team-changed-the-input-type-for-numbers/
- https://bradfrost.com/blog/post/you-probably-dont-need-input-typenumber/
- https://stackoverflow.blog/2022/09/15/why-the-number-input-is-the-worst-input/
- https://ux.stackexchange.com/questions/119870/input-type-number-or-input-type-text-for-entering-an-id


