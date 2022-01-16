# Dev2022
My first Homework HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=>, initial-scale=1.0">
    <title>Jeremy's Blog</title>
</head>
<body>
    <header>
        <span>
            <h1>Rules for Autocomplete</h1>
          <p href="#"><i>Posted on March 19, 2019</i></p><br>
        <input type="text" id="headerSearch" />
      </span>
    </header>
    </nav>
    <aside>
      <nav class="asideNavigation" id="asideNavigation">
        <section class="asideNavigation__internalLinks">
          <p class="asideNavigation__internalLinks__link" href="#">
          Autocompleting text with known values seems like an easy problem to solve, but so so so many UIs get it wrong. I see this frequent enough that, rather than complain about them individuallu, I thought I'd just write down the set of rules they often break.</p><br>
          <p class="asideNavigation__internalLinks__link" href="#">There may be cases where some of these rules aren't the best thing to do, but there should be a good reason for breaking one of these rules (for example, some of these rules don't apply if a field must be filled with a value from a fixed set, like the list of US states). Following these rules should always result in a very least a sane experience:</p><br>
          <ul>
            <li>Exact Matched always come first. If the user types in an opinion exactly, other options must always go below the one matching what they typed.
            </li>
            <li>Besides exact matches, prefix matches come first. If I type "Fr" I want "Fresno" not "San Francisco".
            </li>
            <li>After prefix matches, it can fall back to substring matches. Starting with substring matches would almost always be the wrong thing to do since users start typing workd at the beginning not somewhere in the middle.
            </li>
            <li>If there are no subsequences/substring matches, it can optionaly fall back to approximate matches. This is rarely necessary to provide.
            </li>
            <li>Matches should be sorted alphabetically.
            </li>
            <li>When one option is the prefix of another, put the <i> shortest one first</i>
            </li>
            <li>The matching should probably be case insensitive unless there are two options that differ only by case. In that case(pun intended), prefer the one that more closely matches the user's input.
            </li>
            <li>The action to make use of the selection (e.g. to search the term) must be a different key than the action to accept the first suggestion <i> unless </i> you have to do something first to start autocomplete suggestions(e.g. hit the down arrow). The user should never have to take extra stept to <i> not </i> use autocomplete.
            </li>
          </ul>
 </body>
</html>
