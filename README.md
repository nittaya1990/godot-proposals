# Godot Improvement Proposals

In order to improve the workflow of proposing, discussing, reviewing
and later on implementing features or enhancements in Godot Engine,
this repository is used to centralize all the proposals in one place
apart from bug reports.

Proposals are made by opening issues in this repository, which will
then be discussed with fellow Godot users and contributors. If a
proposal is considered good to implement, it will be approved by a
core developer.

**Proposals should be made by opening an issue, not a pull request.**
Don't fork this repository to open a proposal.

> **Tip:** Use the [Godot proposals viewer](https://godot-proposals-viewer.github.io/)
> to view all open proposals on a single page. This allows for easy searching
> in proposal titles using <kbd>Ctrl + F</kbd>.

## Rules for submitting a proposal

1. Only proposals that properly fill out the template will be considered. If
the template is not filled out or is filled out improperly, it will be closed.

2. Please open one proposal per feature requested. Do not cram multiple feature
requests in a single proposal, as this makes it harder to discuss features
individually.

3. All proposals must be linked to a substantive use-case. In justifying your
proposal, it is not enough to say it would be "nice" or "helpful". Use the
template to show how Godot is not currently meeting your needs and then
explain how your proposal will meet a particular need.
   * If you feel that you cannot provide highly detailed instructions with the
     proposal, consider creating a more simple, open-ended issue in the
     unofficial, community-maintained
     [Godot Ideas](https://github.com/godot-extended-libraries/godot-ideas)
     repository.

4. Other users must express interest in your proposal for it to be considered.
Godot is community-driven: if no other users are interested in your proposal,
it may be closed. It is up to you to draw interest in your proposed feature.
Start by reaching out on the community channels (Reddit, Discord, IRC, etc.
see the [Community Channels](http://docs.godotengine.org/en/stable/community/channels.html) doc),
then create your proposal once you have gained some interest.

5. You can make a PR implementing the feature in the main repository before
making a proposal. However, if it is a large change, a core developer may
require that you make a proposal before your PR can be merged. It is always
better to make and discuss a proposal before spending your time implementing
a new feature.

6. If you or another user is capable of making a PR, include that fact in
the issue or in a subsequent comment so that a core contributor can
fast-track the approval process.

## What to do if your proposal is closed

If your proposal was closed because the template was not filled out, then
fill out the [template](.github/ISSUE_TEMPLATE/feature_enhancement_proposal.yml)
and ask the person who closed the issue to re-open it.

If your proposal was closed as a duplicate and had a different approach to solving
the problem described in the linked proposal, please comment in the linked proposal
with your own proposal. You don't need to copy-paste your whole proposal's text.
Instead, rephrase the main ideas and add mockups if needed.

If your proposal was closed because of lack of interest, then try to build up
some interest on the [community channels](http://docs.godotengine.org/en/stable/community/channels.html)
and then ask the person who closed the issue to re-open it.

If your proposal was closed because a core contributor determined that it was
not worth pursuing and you feel that it was wrongly closed, then feel free
to join the developer IRC channel (`#godotengine-devel` on `irc.freenode.net`)
and have a more in-depth discussion with other core developers about the feature.

## How core developers evaluate proposals

The following is a list of considerations that core developers use when deciding
to accept, close, or leave a proposal open. It is intended to be useful for core
developers when considering proposals and for proposal-makers in drafting their
proposals.

#### 1. Does the proposal comply with the rules?

Read the proposal and check to see that it complies with the above-stated rules.
If it does not, close the proposal.

#### 2. How much support is the proposal receiving?

Evaluate the amount of support the proposal is receiving. This is an ongoing
analysis. If a proposal receives little support at first, it may receive
additional support later on.

#### 3. Can this proposal be implemented with an addon?

Evaluate whether it is possible for the proposal to be implemented in an addon.
If it is possible for the proposal to be in an addon, it is less likely to be
accepted.

#### 4. Does this proposal benefit most users?

Determine whether this proposal benefits all users, or just certain users.
For example, a feature that can only be used for 3D FPS games is less
likely to be accepted than a feature that benefits all 3D games.

#### 5. Can this proposal be implemented in a robust, general-purpose way?

Determine whether the feature can be implemented in a robust way that benefits
all use-cases. For example, many games use an inventory system, but every game
implements inventory differently. Accordingly, a proposal for an inventory
system will likely not be accepted because it would be impossible for us to
implement an inventory system that works for most users that need an inventory
in their game.

#### 6. Does this proposal help users overcome a limitation?

Proposals that overcome a specific limitation are more likely to be accepted
than proposals that are just helpful. In short, need-to-have features will be
prioritized over nice-to-have features. Further, the core developers prioritize
changes that enable users to implement features themselves over implementing
those same features in core.

#### 7. How complex would the proposed feature be?

A highly complex new feature involving substantial changes to core is less likely
to be accepted than a feature that can be contained within a single node, or a
group of nodes.

#### 8. Can the feature be worked around in script with a few lines?

If the feature is only intended to save users a few lines of code it is unlikely
to be accepted.

The above considerations are all balanced, no one is more important than another.
Core developers have discretion to weigh the factors as they see fit.

In addition to the above guideline, consider [this article](https://docs.godotengine.org/en/latest/community/contributing/best_practices_for_engine_contributors.html)
which outlines what core developers consider when evaluating PRs.
