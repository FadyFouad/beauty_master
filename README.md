## Beauty Master App

### Getting Started
This command comes useful when you want to make sure your code is clean and ready to be code-reviewed. it does the
following:

- runs [flutter_gen](https://pub.dev/packages/flutter_gen)
- runs `flutter analyze`


### Fluttergen

We use [Fluttergen](https://pub.dev/packages/flutter_gen) to properly generate index files for our assets, this way all
the paths are saved into constants.

after you install it in your system, you can run the following command:

```bash 
fluttergen -c pubspec.yaml
```

in the root of project to generate `Assets.gen.dart` files and others.

### Flutter analyze
Analyze your code to find potential issues.

```bash
flutter analyze
```


### New libraries

Before adding new libraries to the project, please consult it with the team.  
It's important to keep the project as clean as possible and avoid adding unnecessary dependencies.
it might impose code style, architecture or other limitations that might not be compatible with the project.
And it might make the maintenance much harder. If a solution provided by library is trivial, its better to host the code
inside the project rather than relying on third parties


### Commit messages 
- use imperative, present tense: "change" not "changed" nor "changes"
- don't capitalize first letter
- no dot (.) at the end
- reference issues and pull requests liberally
- when only changing documentation, include [ci skip] in the commit title
- consider starting the commit message with an applicable emoji:

#### examples
- git commit -m 'feat: Add user profile picture upload functionality'
- git commit -m 'fix: User profile picture upload not working'
- git commit -m 'docs: Correct spelling of CHANGELOG'
- git commit -m 'refactor: User profile picture upload'
- git commit -m 'test: Add user profile picture upload test'
- git commit -m 'chore: Run tests on Travis CI'
- git commit -m 'style: Format code according to coding guidelines'
- git commit -m 'ci: Add Travis CI build status badge to README'
- git commit -m 'perf: Improve user profile picture upload speed'
- git commit -m 'revert: Revert previous commit that caused issues'
- git commit -m 'ci: Integrate automated testing into continuous integration pipeline'

// TODO