This file is part of DecimalsRangeRegexpGenerator.

DecimalsRangeRegexpGenerator is free software:
you can redistribute it and/or modify it
under the terms of the GNU Affero General Public License
as published by the Free Software Foundation,
either version 3 of the License,
or (at your option) any later version.

DecimalsRangeRegexpGenerator is distributed in the hope
that it will be useful, but WITHOUT ANY WARRANTY;
without even the implied warranty of MERCHANTABILITY
or FITNESS FOR A PARTICULAR PURPOSE.
See the GNU Affero General Public License for more details.

You should have received a copy of the
GNU Affero General Public License
along with DecimalsRangeRegexpGenerator.
If not, see <https://www.gnu.org/licenses/>

©Copyright 2022 Laurent Lyaudet

# DecimalsRangeRegexpGenerator
Handle min, max and step to produce a regular expression
for ranges of decimal numbers.

Several integers range regular expression generators
can be found on GitHub,
but they do not handle decimal numbers.
(Decimal numbers are the subset of the rational numbers
that can be written as n/10^k where n and k are integers.)
They can handle min and max parameters,
but they do not handle step parameter.

The goal of this dev tool is to have an easy path
to avoid most use cases of HTML's:

    <input type="number" min="@some_decimal1@" max="@some_decimal2@" step="@some_decimal3@">

by using

    <input type="text" inputmode="numeric" pattern="@some_regexp@">

instead.

For a few reasons to replace input number
with input text and a pattern,
you may read the following blog articles or webpages:
- https://technology.blog.gov.uk/2020/02/24/why-the-gov-uk-design-system-team-changed-the-input-type-for-numbers/
- https://bradfrost.com/blog/post/you-probably-dont-need-input-typenumber/
- https://stackoverflow.blog/2022/09/15/why-the-number-input-is-the-worst-input/
- https://ux.stackexchange.com/questions/119870/input-type-number-or-input-type-text-for-entering-an-id
