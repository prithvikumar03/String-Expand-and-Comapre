# String-Expand-and-Comapre
Expand string according to a set of rules and then search for a given string

std::string PatternSearch(const unsigned char* pStr, const unsigned char* pMatch)

{

    // This function searches given null terminated string pStr by given subset of regular expression pMatch.

    // Return value is matched string appeared in pStr.

    // If nothing has matched, return value is empty string.

    //

    // The subset of regular expression grammar is defined as follows.

    //   - A string is set of 8-bit characters. Beware that it is not 7-bit.

    //   - The metacharacter \ is an escape character, that means any single letter appeared next used as is.

    //   - The characters in squared brackets metacharacters [ and ] is a sequence of literal characters or metacharacters.

    //     Immediately after ], another metacharacters in curly braces { num } must be followed. The num is a sequence of

    //     digits which specifies the number of times the previous literal character or metacharacter sequence in squared

    //     brackets must be repeated.

    //     e.g. "abc[def]{2}ghi" matches "abcdefdefghi".

    //   - The squared brackets metacharacters can be nested.

    //     e.g. "abc[def[ghi]{3}jkl]{2}mno matches "abcdefghighighijkldefghighighijklmno".

    //   - In case of matching pattern given by pMatch is a grammatical error, this function returns a string "ERROR".

    //

}

The function only returns matched string once.

e.g. . pStr:”abcdeabc abcffaaa”, pMatch:”abc”, output:”abc”
