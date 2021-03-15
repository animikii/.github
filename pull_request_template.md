# {Jira Ticket#}: Pull-Request Title

* Please create one pull-request per Jira ticket.
* Start the pull-request title with the Jira ticket number followed by the ticket title. This will provide valuable context to the reviewer. Example: `SN-42: As a developer, I need to create and run a script to update video embed codes on courses`.
* If this pull-request is a work in progress (ready for feedback, but not ready to be merged), prepend `WIP: ` to the title and mark it as a draft. Don't forget to update the title when it's ready to be merged.

The purpose of this pull-request. _What_ does this pull-request do? _Why_ does it do it?


---

# Conforms to Style Guides

## [Ruby code](https://styleguide.animikii.com/ruby)

- [ ] Use [AKII's Rubocop config](https://github.com/animikii/rubocop-akii) and clear all warnings.
- [ ] Use [YARD comments](https://yardoc.org) for all methods/classes

## [Rails](https://styleguide.animikii.com/ruby/rails)

- [ ] Validation syntax (e.g. `validates :title, presence: true`)
- [ ] Pundit-style permissions
- [ ] `BaseController` for each namespace

## [GIT](https://styleguide.animikii.com/git)

- Commit messages
  - [ ] Imperative, present-tense (should be phrased like you are finishing the sentence, “When applied, this commit will _[commit message]_”)
    - First line is subject-line-like
      - [ ] About 50 characters or less
        - [ ] Sentence-case, no terminating period
        - [ ] Grammatically correct
      - Any subsequent lines are:
      - [ ] separated from the first line by a blank line
        - [ ] wrapped at 72 characters

## [React](https://styleguide.animikii.com/react)

- [ ] Pure functions — no side-effects
- [ ] Use classes for reusable objects
- [ ] Maintain immutable data
- Just use [Prettier](https://prettier.io), already!
  - [ ] No trailing white-space
    - [ ] Use semicolons
    - [ ] 80 characters per line
    - [ ] One component per file
  - [ ] Always use JSX format

## [CSS/SASS](https://styleguide.animikii.com/sass)

- CSS
  - [ ] Two spaces for indentation
    - [ ] Prefer dashes over camel-casing
    - [ ] Don't use ID selectors
    - [ ] One selector per line when using multiple selectors
    - [ ] Put a space before the opening brace
    - [ ] Put the closing brace on a new line
    - [ ] Blank lines between rule declarations
    - [ ] OOCSS/BEM/SUIT
    - [ ] Don't use [`!important?`](https://uxengineer.com/css-specificity-avoid-important-css/)
    - SASS
  - [ ] SCSS syntax
    - [ ] Regular properties first
    - [ ] `@include`s second
    - [ ] Nested selectors third
    - [ ] Dashes for variables
    - [ ] Don't nest selectors more than three levels deep
    - Using Bootstrap?
  - [ ] Use utility classes as much as possible
    - [ ] Consistently use mobile-first methodology (min-width media queries)

# Added/removed dependencies

- Gems?
- Node modules?
- Other?
- Why were they added/removed?
- Why were those specific packages chosen?

# Database

- Migrations are reversible?
- Changes existing data?
- Dropping a table/column?
- Document commands that devs need to run after this update (e.g. `rake db:seeds`)
- Is the database/data being migrated in multiple stages?
  - See https://github.com/animikii/ahslovit-web/pull/46
    - Document what all the stages will look like

# Documentation

- Does your change require the docs to be updated?
- Does this PR include the doc update, or have you created a task to do this?

# Additional information for reviewer(s)

- Any caveats?
- Things you considered, but didn't do and why
- Side-effects, dangers of this PR
- To-do's/hacks/technical debt in this PR needing future attention

# Linked resources

- Jira ticket
- @mentions
- Slack conversations
- GitHub issue
- Related pull-requests
