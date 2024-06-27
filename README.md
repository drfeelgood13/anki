# Report for Assignment 1

## Project chosen

Name: Anki

URL: https://github.com/drfeelgood13/anki

Number of lines of code and the tool used to count it: 113.385 LOC, Lizard

Programming language: Python

## Coverage measurement

### Existing tool

<Inform the name of the existing tool that was executed and how it was executed>
The name of the existing tool we used is “Coverage.py”. We opened the project and checked if we had Python 3 installed. Some of us didn’t, so we installed the latest version of Python. Then we installed the tool using the following command: $ python3 -m pip install coverage. We then went to the wanted directory to check the coverage for, which is /anki/pylib/tests, and then ran the coverage test using the following command: $ coverage run -m pytest. Afterward, we used the command: $ coverage html to get the coverage report formatted nicely. In the end, we opened the report page from “htmlcov/index.html”. 

After we executed the tool, we used the results to identify the poorly tested methods that need to be improved by us.

<Show the coverage results provided by the existing tool with a screenshot>
	
![totalrep1](https://github.com/drfeelgood13/anki/assets/122294492/056c5d64-e5e1-474f-9d55-ada6d4cc1898)
	
![totalrep2](https://github.com/drfeelgood13/anki/assets/122294492/fe36818c-8112-44e7-8b0d-471c333f447f)

![totalrep3](https://github.com/drfeelgood13/anki/assets/122294492/23f21f03-a613-4479-8251-f7b01b8aa67a)

![totalrep4](https://github.com/drfeelgood13/anki/assets/122294492/d5900ff3-9129-44ec-aea1-b1ff793d31cd)

### Your own coverage tool

Rafael Haenel Musa

<Function 1 name>

	DeckManager.card_count

<Show a patch (diff) or a link to a commit made in your forked repository that shows the instrumented code to gather coverage measurements>

https://github.com/ankitects/anki/compare/main...drfeelgood13:anki:rafael

<Provide a screenshot of the coverage results output by the instrumentation>
	
![rafa1](https://github.com/drfeelgood13/anki/assets/122294492/146bdf38-28aa-4806-96a3-632f0e9632dd)

<Function 2 name>
DeckManager.add_normal_deck_with_name

<Show a patch (diff) or a link to a commit made in your forked repository that shows the instrumented code to gather coverage measurements>
	https://github.com/ankitects/anki/compare/main...drfeelgood13:anki:rafael

<Provide a screenshot of the coverage results output by the instrumentation>
	
	![rafa2](https://github.com/drfeelgood13/anki/assets/122294492/209031fb-2c27-42ce-beaa-7181f0187462)

	
Vlad Parau

<Function 1 name>
Collection.sched_ver

<Show a patch (diff) or a link to a commit made in your forked repository that shows the instrumented code to gather coverage measurements>
https://github.com/ankitects/anki/commit/16be6169707fe02b991cef26d73e3b64c0f5616e

<Provide a screenshot of the coverage results output by the instrumentation>
	
![vlad1](https://github.com/drfeelgood13/anki/assets/122294492/79a214d9-9920-44ba-934f-6072f48619ac)

<Function 2 name>
BrowserConfig.sort_column_key

<Show a patch (diff) or a link to a commit made in your forked repository that shows the instrumented code to gather coverage measurements>
https://github.com/ankitects/anki/commit/a7813812749d55efe6dcdfac6106c64816af8824

<Provide a screenshot of the coverage results output by the instrumentation>
	
![vlad2](https://github.com/drfeelgood13/anki/assets/122294492/09543bbb-69fa-424b-bd23-60aea4eb27a3)

Isabela Aterman

<Function 1 name>
capitalcase

<Show a patch (diff) or a link to a commit made in your forked repository that shows the instrumented code to gather coverage measurements>
https://github.com/drfeelgood13/anki/commit/dd2dc9836b58607cc5d0ba575f772eb337a2050b

<Provide a screenshot of the coverage results output by the instrumentation>
	
![isa1](https://github.com/drfeelgood13/anki/assets/122294492/f5d4fdab-256a-4eec-b51c-284826394baa)

<Function 2 name>
camelcase

<Show a patch (diff) or a link to a commit made in your forked repository that shows the instrumented code to gather coverage measurements>
https://github.com/drfeelgood13/anki/commit/247fbe0d32928b7280e53d7c9eff536d0a39c1b2

<Provide a screenshot of the coverage results output by the instrumentation>
	
![isa2](https://github.com/drfeelgood13/anki/assets/122294492/f1907557-b7a1-45f8-917f-730f2f164707)

Lukas Jokubauskas

<Function 1 name>
_legacy_bulk_add

<Show a patch (diff) or a link to a commit made in your forked repository that shows the instrumented code to gather coverage measurements>
https://github.com/ankitects/anki/commit/ac9c6ac103117792340892757378ed0a1717c62c
<Provide a screenshot of the coverage results output by the instrumentation>

![lukas1](https://github.com/drfeelgood13/anki/assets/122294492/dbe376fd-eae0-4f81-bf89-328da101b14d)

<Function 2 name>
pathcase
<Show a patch (diff) or a link to a commit made in your forked repository that shows the instrumented code to gather coverage measurements>
https://github.com/ankitects/anki/commit/4432cc229aa721831c310e3e4ef19acb300fbbf2

<Provide a screenshot of the coverage results output by the instrumentation>
	
![lukas2](https://github.com/drfeelgood13/anki/assets/122294492/87eab88d-0a18-4570-b683-f19f12e172d5)

## Coverage improvement

### Individual tests

Rafael Hanael Musa

<Test 1 and 2>Both test were made in the same test file for making it easier
	test_decks.py

<Show a patch (diff) or a link to a commit made in your forked repository that shows the new/enhanced test>
https://github.com/ankitects/anki/compare/main...drfeelgood13:anki:rafael

<Provide a screenshot of the old coverage results (the same as you already showed above)>

![rafa3](https://github.com/drfeelgood13/anki/assets/122294492/de8f9bab-f0c3-41aa-941e-ebabb39fad65)

<Provide a screenshot of the new coverage results>
	
![rafa4](https://github.com/drfeelgood13/anki/assets/122294492/4e096b75-70a8-4bdd-9a72-f4b60b5aae69)

<State the coverage improvement with a number and elaborate on why the coverage is improved>
Coverage went from 0% to 100% in both the functions because none of them were accessed on any test before. Just by accessing them I could make big progress on improving the coverage, however some conditions had to be met so I could get the full coverage of that function. The function DeckManager.add_normal_deck_with_name had a condition of creating a deck with a repeated name. The other function DeckManager.card_count had some conditions regarding how the deck parameter was called and if it should include its subdecks. I simply called those functions multiple times each time going through one of those conditions.

Vlad Parau

<Test 1>
test_collection.py

<Show a patch (diff) or a link to a commit made in your forked repository that shows the new/enhanced test>
https://github.com/ankitects/anki/commit/16be6169707fe02b991cef26d73e3b64c0f5616e

<Provide a screenshot of the old coverage results (the same as you already showed above)>

	![vlad3](https://github.com/drfeelgood13/anki/assets/122294492/5d6e3465-d24d-4f55-80e9-8b857d2bec42)

<Provide a screenshot of the new coverage results>
	
![vlad4](https://github.com/drfeelgood13/anki/assets/122294492/7f9e8f5d-e5de-4499-a05f-4e98fb763e3e)

<State the coverage improvement with a number and elaborate on why the coverage is improved>
As illustrated by the screenshots above, the coverage improvement increased by 25%. The initial uncovered part was related to the branch reached only when sched_ver() received an incompatible version of the app’s scheduler as input. In this case, the only compatible versions are 1 and 2. Since the first branch was already covered, I wrote a test for the branch that raised an exception. The test simply creates a configuration that has the third version(the only existing one that is incompatible) of the scheduler and calls sched_ver(). More than that, it is built to expect an assertion. If the assertion isn’t raised, then there might be a problem with the code.

<Test 2>
test_browser.py 

<Show a patch (diff) or a link to a commit made in your forked repository that shows the new/enhanced test>
https://github.com/ankitects/anki/commit/a7813812749d55efe6dcdfac6106c64816af8824
<Provide a screenshot of the old coverage results (the same as you already showed above)>

![vlad5](https://github.com/drfeelgood13/anki/assets/122294492/4997c4e2-e3bd-473a-b659-034ccd7b99d5)

<Provide a screenshot of the new coverage results> 
	
![vlad6](https://github.com/drfeelgood13/anki/assets/122294492/00085ab3-91df-4423-983c-2bd8586c70ba)

<State the coverage improvement with a number and elaborate on why the coverage is improved>
The coverage improvement increased by 100%. The reason why this happened is because none of the method’s branches were covered. The test behind this method is simple, I have just used the only two possible inputs that can occur, namely True and False. When the input is True, it means that the user is in “notes mode” and the test needs to check that this is indeed true, a functionality that was easily implemented using an assert. The other case occurs when the user is in “cards mode”, which will influence the sorting part differently, an aspect checked by another assert. 

Isabela Aterman

<Test 1>
test_cases.py

<Show a patch (diff) or a link to a commit made in your forked repository that shows the new/enhanced test>
https://github.com/drfeelgood13/anki/commit/dd2dc9836b58607cc5d0ba575f772eb337a2050b

<Provide a screenshot of the old coverage results (the same as you already showed above)>

![isa3](https://github.com/drfeelgood13/anki/assets/122294492/f94ef272-80c0-49bc-a341-f45fd9d619ce)

<Provide a screenshot of the new coverage results>
	
![isa4](https://github.com/drfeelgood13/anki/assets/122294492/4e79f254-119e-4e06-a9dc-ce5601abd5b6)

<State the coverage improvement with a number and elaborate on why the coverage is improved>
The coverage of the function went from 0% to 100%. It is improved because now every branch of the method is covered by tests. The chosen function transforms the first character of a string to uppercase, or returns immediately if the input string is empty.  As mentioned before, the input that can occur is either an empty string, or a non-empty string. Thus, I created two asserts in which I check if the output of the function is as expected or not. 

<Test 2>
test_cases.py

https://github.com/drfeelgood13/anki/commit/247fbe0d32928b7280e53d7c9eff536d0a39c1b2

![isa5](https://github.com/drfeelgood13/anki/assets/122294492/099cbc09-018d-49ba-93b3-df8464410872)

![isa6](https://github.com/drfeelgood13/anki/assets/122294492/bea2fd48-778d-4256-a212-5c1a38c11a04)

The function had 0% coverage before. After I added tests for each branch, the coverage improved to 100%. The chosen method transforms strings to camel case, unless the input string is empty and it returns immediately. In order to test the branches, I created two asserts which check if the output of the function is as expected. 


Lukas Jokubauskas

<Test 1>

<Show a patch (diff) or a link to a commit made in your forked repository that shows the new/enhanced test>
https://github.com/ankitects/anki/commit/ac9c6ac103117792340892757378ed0a1717c62c

<Provide a screenshot of the old coverage results (the same as you already showed above)>

![lukas3](https://github.com/drfeelgood13/anki/assets/122294492/f6174293-5fa6-46a0-97bc-370d48b1c4ac)

<Provide a screenshot of the new coverage results>
	
![lukas4](https://github.com/drfeelgood13/anki/assets/122294492/22eb8b91-07fb-4694-9fd1-bf085e4d1e18)

<State the coverage improvement with a number and elaborate on why the coverage is improved>
Coverage improved from 0% to 100%. It has improved because _legacy_bulk_add function takes an array ids and tags and depending on boolean value it either adds multiple tags or removes them and I have tested the function with mock ids and tags both when boolean is true and when it is false and captured whether correct branches are entered in both cases. So all branches are tested now and none were before.

<Test 2>
<Provide the same kind of information provided for Test 1>

https://github.com/ankitects/anki/commit/4432cc229aa721831c310e3e4ef19acb300fbbf2

![lukas5](https://github.com/drfeelgood13/anki/assets/122294492/4ce465bc-8841-4527-bc37-b761c66f9ee1)

![lukas6](https://github.com/drfeelgood13/anki/assets/122294492/e3b26f80-51c4-443d-a8ec-0882b65c8a0f)

Coverage improved from 0% to 100%. Coverage improved because both statements were tested, when the given string is empty and not empty. When given string is not empty it was successfully converted first to snakecase and the to pathcase which assertions confirm. Previously none of the statements were tested and now all statements are tested.

### Overall

<Provide a screenshot of the old coverage results by running an existing tool (the same as you already showed above)>

![totalrep1](https://github.com/drfeelgood13/anki/assets/122294492/19545770-8e5e-4c7f-8a3b-59c82afdca02)

![totalrep2](https://github.com/drfeelgood13/anki/assets/122294492/92a10b2b-ab0e-4332-a625-1c101e6811a4)

![totalrep3](https://github.com/drfeelgood13/anki/assets/122294492/408bffb1-d047-4716-9f89-308a49f45bbd)

![totalrep4](https://github.com/drfeelgood13/anki/assets/122294492/4dc2aad2-2a75-4507-be56-6f3b97f93f85)

<Provide a screenshot of the new coverage results by running the existing tool using all test modifications made by the group>

## Statement of individual contributions

<Write what each group member did>
Vlad improved the coverage of Collection.sched_ver() and BrowserConfig.sort_column_key() and instrumented them at the same time. Besides this, he wrote his parts in the report and configured the environment for testing the methods.

Isabela improved the coverage of camelcase() and capitalcase() and instrumented them at the same time. Besides this, she wrote her parts in the report and the paragraph about the existing coverage tool that we used initially.

Rafael improved the coverage of DeckManager.add_normal_deck_with_name() and DeckManager.card_count() and instrumented them at the same time.

Lukas instrumented and tested _legacy_bulk_add() and pathcase() functions which improved their coverage to 100% and wrote his part of the report.
