<!--- Generated 2018-06-09 at 11:52:24 EDT. Use `./gradlew :meta:update` to update. DO NOT MODIFY DIRECTLY -->

Endpoints
=========

This file contains a list of all the endpoints (regardless of if they have been implemented) that can be found at the [official reddit API docs](https://www.reddit.com/dev/api/oauth). To update this file, run `./gradlew :meta:update`

So far, API completion is at **49.45%**. 90 out of 182 endpoints (ignoring 7 endpoints not planned) have been implemented 

(any scope)
-----------

25.00% completion (1 implemented, 4 planned, and 1 not planned)

| Method | Endpoint                                                                                     | Implementation                                                                                                                                       |
|:------:| -------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| `POST` | [`/api/comment`](https://www.reddit.com/dev/api/oauth#POST_api_comment)                      | [`ReplyableReference.reply()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/ReplyableReference.kt#L14) |
| `POST` | [`[/r/{subreddit}]/api/friend`](https://www.reddit.com/dev/api/oauth#POST_api_friend)        | None                                                                                                                                                 |
| `POST` | [`[/r/{subreddit}]/api/unfriend`](https://www.reddit.com/dev/api/oauth#POST_api_unfriend)    | None                                                                                                                                                 |
| `GET`  | [`/api/username_available`](https://www.reddit.com/dev/api/oauth#GET_api_username_available) | None                                                                                                                                                 |
| `GET`  | [`/api/v1/scopes`](https://www.reddit.com/dev/api/oauth#GET_api_v1_scopes)                   | None                                                                                                                                                 |
| `GET`  | [`/api/needs_captcha`](https://www.reddit.com/dev/api/oauth#GET_api_needs_captcha)           | Not planned                                                                                                                                          |

account
-------

50.00% completion (1 implemented, 1 planned, and 0 not planned)

| Method  | Endpoint                                                                         | Implementation                                                                                                                                           |
|:-------:| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `PATCH` | [`/api/v1/me/prefs`](https://www.reddit.com/dev/api/oauth#PATCH_api_v1_me_prefs) | [`SelfUserReference.patchPrefs()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SelfUserReference.kt#L203) |
| `POST`  | [`/api/block_user`](https://www.reddit.com/dev/api/oauth#POST_api_block_user)    | None                                                                                                                                                     |

creddits
--------

0.00% completion (0 implemented, 2 planned, and 0 not planned)

| Method | Endpoint                                                                                                | Implementation |
|:------:| ------------------------------------------------------------------------------------------------------- | -------------- |
| `POST` | [`/api/v1/gold/gild/{fullname}`](https://www.reddit.com/dev/api/oauth#POST_api_v1_gold_gild_{fullname}) | None           |
| `POST` | [`/api/v1/gold/give/{username}`](https://www.reddit.com/dev/api/oauth#POST_api_v1_gold_give_{username}) | None           |

edit
----

100.00% completion (5 implemented, 0 planned, and 0 not planned)

| Method | Endpoint                                                                                                        | Implementation                                                                                                                                                                |
|:------:| --------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `POST` | [`/api/del`](https://www.reddit.com/dev/api/oauth#POST_api_del)                                                 | [`PublicContributionReference.delete()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/PublicContributionReference.kt#L92)       |
| `POST` | [`/api/editusertext`](https://www.reddit.com/dev/api/oauth#POST_api_editusertext)                               | [`PublicContributionReference.edit()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/PublicContributionReference.kt#L101)        |
| `POST` | [`/api/live/{thread}/delete_update`](https://www.reddit.com/dev/api/oauth#POST_api_live_{thread}_delete_update) | [`LiveThreadReference.deleteUpdate()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/LiveThreadReference.kt#L78)                 |
| `POST` | [`/api/live/{thread}/strike_update`](https://www.reddit.com/dev/api/oauth#POST_api_live_{thread}_strike_update) | [`LiveThreadReference.strikeUpdate()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/LiveThreadReference.kt#L73)                 |
| `POST` | [`/api/sendreplies`](https://www.reddit.com/dev/api/oauth#POST_api_sendreplies)                                 | [`PublicContributionReference.sendReplies()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/PublicContributionReference.kt#L114) |

flair
-----

71.43% completion (5 implemented, 2 planned, and 0 not planned)

| Method | Endpoint                                                                                                | Implementation                                                                                                                                                          |
|:------:| ------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `POST` | [`[/r/{subreddit}]/api/flairselector`](https://www.reddit.com/dev/api/oauth#POST_api_flairselector)     | [`UserFlairReference.current()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/UserFlairReference.kt#L129)                 |
| `GET`  | [`[/r/{subreddit}]/api/link_flair`](https://www.reddit.com/dev/api/oauth#GET_api_link_flair)            | [`SubredditReference.linkFlairOptions()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L169)        |
| `POST` | [`[/r/{subreddit}]/api/selectflair`](https://www.reddit.com/dev/api/oauth#POST_api_selectflair)         | [`FlairReference.updateToTemplate()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/FlairReference.kt#L-1)                 |
| `POST` | [`[/r/{subreddit}]/api/setflairenabled`](https://www.reddit.com/dev/api/oauth#POST_api_setflairenabled) | [`SelfUserFlairReference.setFlairEnabled()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SelfUserFlairReference.kt#L177) |
| `GET`  | [`[/r/{subreddit}]/api/user_flair`](https://www.reddit.com/dev/api/oauth#GET_api_user_flair)            | [`SubredditReference.userFlairOptions()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L160)        |
| `GET`  | [`[/r/{subreddit}]/api/link_flair_v2`](https://www.reddit.com/dev/api/oauth#GET_api_link_flair_v2)      | None                                                                                                                                                                    |
| `GET`  | [`[/r/{subreddit}]/api/user_flair_v2`](https://www.reddit.com/dev/api/oauth#GET_api_user_flair_v2)      | None                                                                                                                                                                    |

history
-------

100.00% completion (1 implemented, 0 planned, and 0 not planned)

| Method | Endpoint                                                                                       | Implementation                                                                                                                               |
|:------:| ---------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| `GET`  | [`/user/{username}/{where}`](https://www.reddit.com/dev/api/oauth#GET_user_{username}_{where}) | [`UserReference.history()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/UserReference.kt#L84) |

identity
--------

100.00% completion (3 implemented, 0 planned, and 0 not planned)

| Method | Endpoint                                                                             | Implementation                                                                                                                                      |
|:------:| ------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| `GET`  | [`/api/v1/me`](https://www.reddit.com/dev/api/oauth#GET_api_v1_me)                   | [`UserReference.query()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/UserReference.kt#L39)          |
| `GET`  | [`/api/v1/me/prefs`](https://www.reddit.com/dev/api/oauth#GET_api_v1_me_prefs)       | [`SelfUserReference.prefs()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SelfUserReference.kt#L189) |
| `GET`  | [`/api/v1/me/trophies`](https://www.reddit.com/dev/api/oauth#GET_api_v1_me_trophies) | [`UserReference.trophies()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/UserReference.kt#L54)       |

livemanage
----------

20.00% completion (2 implemented, 8 planned, and 0 not planned)

| Method | Endpoint                                                                                                                                    | Implementation                                                                                                                                         |
|:------:| ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `POST` | [`/api/live/{thread}/close_thread`](https://www.reddit.com/dev/api/oauth#POST_api_live_{thread}_close_thread)                               | [`LiveThreadReference.close()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/LiveThreadReference.kt#L97) |
| `POST` | [`/api/live/{thread}/edit`](https://www.reddit.com/dev/api/oauth#POST_api_live_{thread}_edit)                                               | [`LiveThreadReference.edit()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/LiveThreadReference.kt#L53)  |
| `POST` | [`/api/live/{thread}/accept_contributor_invite`](https://www.reddit.com/dev/api/oauth#POST_api_live_{thread}_accept_contributor_invite)     | None                                                                                                                                                   |
| `POST` | [`/api/live/{thread}/hide_discussion`](https://www.reddit.com/dev/api/oauth#POST_api_live_{thread}_hide_discussion)                         | None                                                                                                                                                   |
| `POST` | [`/api/live/{thread}/invite_contributor`](https://www.reddit.com/dev/api/oauth#POST_api_live_{thread}_invite_contributor)                   | None                                                                                                                                                   |
| `POST` | [`/api/live/{thread}/leave_contributor`](https://www.reddit.com/dev/api/oauth#POST_api_live_{thread}_leave_contributor)                     | None                                                                                                                                                   |
| `POST` | [`/api/live/{thread}/rm_contributor`](https://www.reddit.com/dev/api/oauth#POST_api_live_{thread}_rm_contributor)                           | None                                                                                                                                                   |
| `POST` | [`/api/live/{thread}/rm_contributor_invite`](https://www.reddit.com/dev/api/oauth#POST_api_live_{thread}_rm_contributor_invite)             | None                                                                                                                                                   |
| `POST` | [`/api/live/{thread}/set_contributor_permissions`](https://www.reddit.com/dev/api/oauth#POST_api_live_{thread}_set_contributor_permissions) | None                                                                                                                                                   |
| `POST` | [`/api/live/{thread}/unhide_discussion`](https://www.reddit.com/dev/api/oauth#POST_api_live_{thread}_unhide_discussion)                     | None                                                                                                                                                   |

modconfig
---------

20.00% completion (2 implemented, 8 planned, and 0 not planned)

| Method | Endpoint                                                                                                          | Implementation                                                                                                                                                   |
|:------:| ----------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `POST` | [`[/r/{subreddit}]/api/subreddit_stylesheet`](https://www.reddit.com/dev/api/oauth#POST_api_subreddit_stylesheet) | [`SubredditReference.updateStylesheet()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L226) |
| `GET`  | [`[/r/{subreddit}]/stylesheet`](https://www.reddit.com/dev/api/oauth#GET_stylesheet)                              | [`SubredditReference.stylesheet()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L213)       |
| `POST` | [`[/r/{subreddit}]/api/delete_sr_banner`](https://www.reddit.com/dev/api/oauth#POST_api_delete_sr_banner)         | None                                                                                                                                                             |
| `POST` | [`[/r/{subreddit}]/api/delete_sr_header`](https://www.reddit.com/dev/api/oauth#POST_api_delete_sr_header)         | None                                                                                                                                                             |
| `POST` | [`[/r/{subreddit}]/api/delete_sr_icon`](https://www.reddit.com/dev/api/oauth#POST_api_delete_sr_icon)             | None                                                                                                                                                             |
| `POST` | [`[/r/{subreddit}]/api/delete_sr_img`](https://www.reddit.com/dev/api/oauth#POST_api_delete_sr_img)               | None                                                                                                                                                             |
| `POST` | [`/api/site_admin`](https://www.reddit.com/dev/api/oauth#POST_api_site_admin)                                     | None                                                                                                                                                             |
| `POST` | [`[/r/{subreddit}]/api/upload_sr_img`](https://www.reddit.com/dev/api/oauth#POST_api_upload_sr_img)               | None                                                                                                                                                             |
| `GET`  | [`/r/{subreddit}/about/edit`](https://www.reddit.com/dev/api/oauth#GET_r_{subreddit}_about_edit)                  | None                                                                                                                                                             |
| `GET`  | [`/r/{subreddit}/about/traffic`](https://www.reddit.com/dev/api/oauth#GET_r_{subreddit}_about_traffic)            | None                                                                                                                                                             |

modcontributors
---------------

0.00% completion (0 implemented, 2 planned, and 0 not planned)

| Method | Endpoint                                                                                            | Implementation |
|:------:| --------------------------------------------------------------------------------------------------- | -------------- |
| `POST` | [`/api/mute_message_author`](https://www.reddit.com/dev/api/oauth#POST_api_mute_message_author)     | None           |
| `POST` | [`/api/unmute_message_author`](https://www.reddit.com/dev/api/oauth#POST_api_unmute_message_author) | None           |

modflair
--------

30.00% completion (3 implemented, 7 planned, and 0 not planned)

| Method  | Endpoint                                                                                                           | Implementation                                                                                                                                                 |
|:-------:| ------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `POST`  | [`[/r/{subreddit}]/api/flair`](https://www.reddit.com/dev/api/oauth#POST_api_flair)                                | [`FlairReference.updateToCssClass()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/FlairReference.kt#L-1)        |
| `POST`  | [`[/r/{subreddit}]/api/flaircsv`](https://www.reddit.com/dev/api/oauth#POST_api_flaircsv)                          | [`SubredditReference.patchFlairList()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L254) |
|  `GET`  | [`[/r/{subreddit}]/api/flairlist`](https://www.reddit.com/dev/api/oauth#GET_api_flairlist)                         | [`SubredditReference.flairList()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L242)      |
| `POST`  | [`[/r/{subreddit}]/api/clearflairtemplates`](https://www.reddit.com/dev/api/oauth#POST_api_clearflairtemplates)    | None                                                                                                                                                           |
| `POST`  | [`[/r/{subreddit}]/api/deleteflair`](https://www.reddit.com/dev/api/oauth#POST_api_deleteflair)                    | None                                                                                                                                                           |
| `POST`  | [`[/r/{subreddit}]/api/deleteflairtemplate`](https://www.reddit.com/dev/api/oauth#POST_api_deleteflairtemplate)    | None                                                                                                                                                           |
| `PATCH` | [`[/r/{subreddit}]/api/flair_template_order`](https://www.reddit.com/dev/api/oauth#PATCH_api_flair_template_order) | None                                                                                                                                                           |
| `POST`  | [`[/r/{subreddit}]/api/flairconfig`](https://www.reddit.com/dev/api/oauth#POST_api_flairconfig)                    | None                                                                                                                                                           |
| `POST`  | [`[/r/{subreddit}]/api/flairtemplate`](https://www.reddit.com/dev/api/oauth#POST_api_flairtemplate)                | None                                                                                                                                                           |
| `POST`  | [`[/r/{subreddit}]/api/flairtemplate_v2`](https://www.reddit.com/dev/api/oauth#POST_api_flairtemplate_v2)          | None                                                                                                                                                           |

modlog
------

0.00% completion (0 implemented, 1 planned, and 0 not planned)

| Method | Endpoint                                                                           | Implementation |
|:------:| ---------------------------------------------------------------------------------- | -------------- |
| `GET`  | [`[/r/{subreddit}]/about/log`](https://www.reddit.com/dev/api/oauth#GET_about_log) | None           |

modmail
-------

0.00% completion (0 implemented, 16 planned, and 0 not planned)

|  Method  | Endpoint                                                                                                                                             | Implementation |
|:--------:| ---------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- |
|  `POST`  | [`/api/mod/bulk_read`](https://www.reddit.com/dev/api/oauth#POST_api_mod_bulk_read)                                                                  | None           |
|  `GET`   | [`/api/mod/conversations`](https://www.reddit.com/dev/api/oauth#GET_api_mod_conversations)                                                           | None           |
|  `POST`  | [`/api/mod/conversations`](https://www.reddit.com/dev/api/oauth#POST_api_mod_conversations)                                                          | None           |
|  `POST`  | [`/api/mod/conversations/read`](https://www.reddit.com/dev/api/oauth#POST_api_mod_conversations_read)                                                | None           |
|  `GET`   | [`/api/mod/conversations/subreddits`](https://www.reddit.com/dev/api/oauth#GET_api_mod_conversations_subreddits)                                     | None           |
|  `POST`  | [`/api/mod/conversations/unread`](https://www.reddit.com/dev/api/oauth#POST_api_mod_conversations_unread)                                            | None           |
|  `GET`   | [`/api/mod/conversations/unread/count`](https://www.reddit.com/dev/api/oauth#GET_api_mod_conversations_unread_count)                                 | None           |
|  `GET`   | [`/api/mod/conversations/{conversation_id}`](https://www.reddit.com/dev/api/oauth#GET_api_mod_conversations_:conversation_id)                        | None           |
|  `POST`  | [`/api/mod/conversations/{conversation_id}`](https://www.reddit.com/dev/api/oauth#POST_api_mod_conversations_:conversation_id)                       | None           |
|  `POST`  | [`/api/mod/conversations/{conversation_id}/archive`](https://www.reddit.com/dev/api/oauth#POST_api_mod_conversations_:conversation_id_archive)       | None           |
| `DELETE` | [`/api/mod/conversations/{conversation_id}/highlight`](https://www.reddit.com/dev/api/oauth#DELETE_api_mod_conversations_:conversation_id_highlight) | None           |
|  `POST`  | [`/api/mod/conversations/{conversation_id}/highlight`](https://www.reddit.com/dev/api/oauth#POST_api_mod_conversations_:conversation_id_highlight)   | None           |
|  `POST`  | [`/api/mod/conversations/{conversation_id}/mute`](https://www.reddit.com/dev/api/oauth#POST_api_mod_conversations_:conversation_id_mute)             | None           |
|  `POST`  | [`/api/mod/conversations/{conversation_id}/unarchive`](https://www.reddit.com/dev/api/oauth#POST_api_mod_conversations_:conversation_id_unarchive)   | None           |
|  `POST`  | [`/api/mod/conversations/{conversation_id}/unmute`](https://www.reddit.com/dev/api/oauth#POST_api_mod_conversations_:conversation_id_unmute)         | None           |
|  `GET`   | [`/api/mod/conversations/{conversation_id}/user`](https://www.reddit.com/dev/api/oauth#GET_api_mod_conversations_:conversation_id_user)              | None           |

modothers
---------

0.00% completion (0 implemented, 1 planned, and 0 not planned)

| Method | Endpoint                                                                                              | Implementation |
|:------:| ----------------------------------------------------------------------------------------------------- | -------------- |
| `POST` | [`[/r/{subreddit}]/api/setpermissions`](https://www.reddit.com/dev/api/oauth#POST_api_setpermissions) | None           |

modposts
--------

42.86% completion (6 implemented, 8 planned, and 0 not planned)

| Method | Endpoint                                                                                          | Implementation                                                                                                                                                                |
|:------:| ------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `POST` | [`/api/approve`](https://www.reddit.com/dev/api/oauth#POST_api_approve)                           | [`PublicContributionReference.approve()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/PublicContributionReference.kt#L185)     |
| `POST` | [`/api/distinguish`](https://www.reddit.com/dev/api/oauth#POST_api_distinguish)                   | [`PublicContributionReference.distinguish()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/PublicContributionReference.kt#L137) |
| `POST` | [`/api/remove`](https://www.reddit.com/dev/api/oauth#POST_api_remove)                             | [`PublicContributionReference.remove()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/PublicContributionReference.kt#L171)      |
| `POST` | [`/api/set_subreddit_sticky`](https://www.reddit.com/dev/api/oauth#POST_api_set_subreddit_sticky) | [`SubmissionReference.stickyPost()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubmissionReference.kt#L114)                  |
| `POST` | [`/api/spoiler`](https://www.reddit.com/dev/api/oauth#POST_api_spoiler)                           | [`SubmissionReference.flagAsSpoiler()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubmissionReference.kt#L91)                |
| `POST` | [`/api/unspoiler`](https://www.reddit.com/dev/api/oauth#POST_api_unspoiler)                       | [`SubmissionReference.flagAsSpoiler()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubmissionReference.kt#L91)                |
| `POST` | [`/api/ignore_reports`](https://www.reddit.com/dev/api/oauth#POST_api_ignore_reports)             | None                                                                                                                                                                          |
| `POST` | [`/api/lock`](https://www.reddit.com/dev/api/oauth#POST_api_lock)                                 | None                                                                                                                                                                          |
| `POST` | [`/api/marknsfw`](https://www.reddit.com/dev/api/oauth#POST_api_marknsfw)                         | None                                                                                                                                                                          |
| `POST` | [`/api/set_contest_mode`](https://www.reddit.com/dev/api/oauth#POST_api_set_contest_mode)         | None                                                                                                                                                                          |
| `POST` | [`/api/set_suggested_sort`](https://www.reddit.com/dev/api/oauth#POST_api_set_suggested_sort)     | None                                                                                                                                                                          |
| `POST` | [`/api/unignore_reports`](https://www.reddit.com/dev/api/oauth#POST_api_unignore_reports)         | None                                                                                                                                                                          |
| `POST` | [`/api/unlock`](https://www.reddit.com/dev/api/oauth#POST_api_unlock)                             | None                                                                                                                                                                          |
| `POST` | [`/api/unmarknsfw`](https://www.reddit.com/dev/api/oauth#POST_api_unmarknsfw)                     | None                                                                                                                                                                          |

modself
-------

0.00% completion (0 implemented, 3 planned, and 0 not planned)

| Method | Endpoint                                                                                                                | Implementation |
|:------:| ----------------------------------------------------------------------------------------------------------------------- | -------------- |
| `POST` | [`[/r/{subreddit}]/api/accept_moderator_invite`](https://www.reddit.com/dev/api/oauth#POST_api_accept_moderator_invite) | None           |
| `POST` | [`/api/leavecontributor`](https://www.reddit.com/dev/api/oauth#POST_api_leavecontributor)                               | None           |
| `POST` | [`/api/leavemoderator`](https://www.reddit.com/dev/api/oauth#POST_api_leavemoderator)                                   | None           |

modwiki
-------

0.00% completion (0 implemented, 5 planned, and 0 not planned)

| Method | Endpoint                                                                                                              | Implementation |
|:------:| --------------------------------------------------------------------------------------------------------------------- | -------------- |
| `POST` | [`[/r/{subreddit}]/api/wiki/alloweditor/{act}`](https://www.reddit.com/dev/api/oauth#POST_api_wiki_alloweditor_{act}) | None           |
| `POST` | [`[/r/{subreddit}]/api/wiki/hide`](https://www.reddit.com/dev/api/oauth#POST_api_wiki_hide)                           | None           |
| `POST` | [`[/r/{subreddit}]/api/wiki/revert`](https://www.reddit.com/dev/api/oauth#POST_api_wiki_revert)                       | None           |
| `GET`  | [`[/r/{subreddit}]/wiki/settings/{page}`](https://www.reddit.com/dev/api/oauth#GET_wiki_settings_{page})              | None           |
| `POST` | [`[/r/{subreddit}]/wiki/settings/{page}`](https://www.reddit.com/dev/api/oauth#POST_wiki_settings_{page})             | None           |

mysubreddits
------------

66.67% completion (2 implemented, 1 planned, and 0 not planned)

| Method | Endpoint                                                                                                 | Implementation                                                                                                                                           |
|:------:| -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `GET`  | [`/api/v1/me/karma`](https://www.reddit.com/dev/api/oauth#GET_api_v1_me_karma)                           | [`SelfUserReference.karma()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SelfUserReference.kt#L226)      |
| `GET`  | [`/subreddits/mine/{where}`](https://www.reddit.com/dev/api/oauth#GET_subreddits_mine_{where})           | [`SelfUserReference.subreddits()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SelfUserReference.kt#L218) |
| `GET`  | [`/api/v1/me/friends/{username}`](https://www.reddit.com/dev/api/oauth#GET_api_v1_me_friends_{username}) | None                                                                                                                                                     |

privatemessages
---------------

66.67% completion (6 implemented, 4 planned, and 1 not planned)

| Method | Endpoint                                                                                                 | Implementation                                                                                                                                      |
|:------:| -------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| `POST` | [`/api/compose`](https://www.reddit.com/dev/api/oauth#POST_api_compose)                                  | [`InboxReference.compose()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/InboxReference.kt#L40)      |
| `POST` | [`/api/del_msg`](https://www.reddit.com/dev/api/oauth#POST_api_del_msg)                                  | [`InboxReference.delete()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/InboxReference.kt#L137)      |
| `POST` | [`/api/read_all_messages`](https://www.reddit.com/dev/api/oauth#POST_api_read_all_messages)              | [`InboxReference.markAllRead()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/InboxReference.kt#L121) |
| `POST` | [`/api/read_message`](https://www.reddit.com/dev/api/oauth#POST_api_read_message)                        | [`InboxReference.markRead()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/InboxReference.kt#L112)    |
| `POST` | [`/api/unread_message`](https://www.reddit.com/dev/api/oauth#POST_api_unread_message)                    | [`InboxReference.markRead()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/InboxReference.kt#L112)    |
| `GET`  | [`/message/{where}`](https://www.reddit.com/dev/api/oauth#GET_message_{where})                           | [`InboxReference.iterate()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/InboxReference.kt#L28)      |
| `POST` | [`/api/block`](https://www.reddit.com/dev/api/oauth#POST_api_block)                                      | None                                                                                                                                                |
| `POST` | [`/api/collapse_message`](https://www.reddit.com/dev/api/oauth#POST_api_collapse_message)                | None                                                                                                                                                |
| `POST` | [`/api/unblock_subreddit`](https://www.reddit.com/dev/api/oauth#POST_api_unblock_subreddit)              | None                                                                                                                                                |
| `POST` | [`/api/uncollapse_message`](https://www.reddit.com/dev/api/oauth#POST_api_uncollapse_message)            | None                                                                                                                                                |
| `GET`  | [`/api/user_data_by_account_ids`](https://www.reddit.com/dev/api/oauth#GET_api_user_data_by_account_ids) | Not planned                                                                                                                                         |

read
----

69.23% completion (27 implemented, 15 planned, and 3 not planned)

| Method | Endpoint                                                                                                           | Implementation                                                                                                                                                       |
|:------:| ------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `GET`  | [`[/r/{subreddit}]/api/info`](https://www.reddit.com/dev/api/oauth#GET_api_info)                                   | [`RedditClient.lookup()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/RedditClient.kt#L453)                                      |
| `GET`  | [`/api/live/happening_now`](https://www.reddit.com/dev/api/oauth#GET_api_live_happening_now)                       | [`RedditClient.happeningNow()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/RedditClient.kt#L490)                                |
| `GET`  | [`/api/morechildren`](https://www.reddit.com/dev/api/oauth#GET_api_morechildren)                                   | [`CommentNode.loadMore()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/tree/CommentNode.kt#L-1)                                  |
| `GET`  | [`/api/multi/mine`](https://www.reddit.com/dev/api/oauth#GET_api_multi_mine)                                       | [`UserReference.listMultis()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/UserReference.kt#L101)                     |
| `GET`  | [`/api/multi/user/{username}`](https://www.reddit.com/dev/api/oauth#GET_api_multi_user_{username})                 | [`UserReference.listMultis()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/UserReference.kt#L101)                     |
| `GET`  | [`/api/multi/{multipath}`](https://www.reddit.com/dev/api/oauth#GET_api_multi_{multipath})                         | [`MultiredditReference.about()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/MultiredditReference.kt#L47)             |
| `GET`  | [`/api/multi/{multipath}/description`](https://www.reddit.com/dev/api/oauth#GET_api_multi_{multipath}_description) | [`MultiredditReference.description()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/MultiredditReference.kt#L55)       |
| `PUT`  | [`/api/multi/{multipath}/description`](https://www.reddit.com/dev/api/oauth#PUT_api_multi_{multipath}_description) | [`MultiredditReference.updateDescription()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/MultiredditReference.kt#L64) |
| `GET`  | [`/api/multi/{multipath}/r/{srname}`](https://www.reddit.com/dev/api/oauth#GET_api_multi_{multipath}_r_{srname})   | [`MultiredditReference.subredditInfo()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/MultiredditReference.kt#L120)    |
| `POST` | [`/api/search_subreddits`](https://www.reddit.com/dev/api/oauth#POST_api_search_subreddits)                        | [`RedditClient.searchSubredditsByName()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/RedditClient.kt#L308)                      |
| `GET`  | [`/api/v1/user/{username}/trophies`](https://www.reddit.com/dev/api/oauth#GET_api_v1_user_{username}_trophies)     | [`UserReference.trophies()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/UserReference.kt#L54)                        |
| `GET`  | [`/api/v1/{subreddit}/emojis/all`](https://www.reddit.com/dev/api/oauth#GET_api_v1_{subreddit}_emojis_all)         | [`EmojiReference.list()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/EmojiReference.kt#L27)                          |
| `GET`  | [`/best`](https://www.reddit.com/dev/api/oauth#GET_best)                                                           | [`SubredditReference.posts()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L45)                 |
| `GET`  | [`[/r/{subreddit}]/comments/{article}`](https://www.reddit.com/dev/api/oauth#GET_comments_{article})               | [`SubmissionReference.comments()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubmissionReference.kt#L28)            |
| `GET`  | [`[/r/{subreddit}]/hot`](https://www.reddit.com/dev/api/oauth#GET_hot)                                             | [`SubredditReference.posts()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L45)                 |
| `GET`  | [`/live/{thread}`](https://www.reddit.com/dev/api/oauth#GET_live_{thread})                                         | [`LiveThreadReference.latestUpdates()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/LiveThreadReference.kt#L35)       |
| `GET`  | [`/live/{thread}/about`](https://www.reddit.com/dev/api/oauth#GET_live_{thread}_about)                             | [`LiveThreadReference.about()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/LiveThreadReference.kt#L25)               |
| `GET`  | [`[/r/{subreddit}]/new`](https://www.reddit.com/dev/api/oauth#GET_new)                                             | [`SubredditReference.posts()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L45)                 |
| `GET`  | [`/r/{subreddit}/about`](https://www.reddit.com/dev/api/oauth#GET_r_{subreddit}_about)                             | [`SubredditReference.about()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L30)                 |
| `GET`  | [`/r/{subreddit}/about/rules`](https://www.reddit.com/dev/api/oauth#GET_r_{subreddit}_about_rules)                 | [`SubredditReference.rules()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L202)                |
| `GET`  | [`[/r/{subreddit}]/random`](https://www.reddit.com/dev/api/oauth#GET_random)                                       | [`RedditClient.randomSubreddit()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/RedditClient.kt#L383)                             |
| `GET`  | [`[/r/{subreddit}]/rising`](https://www.reddit.com/dev/api/oauth#GET_rising)                                       | [`SubredditReference.posts()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L45)                 |
| `GET`  | [`[/r/{subreddit}]/search`](https://www.reddit.com/dev/api/oauth#GET_search)                                       | [`SearchPaginator.createNextRequest()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/pagination/SearchPaginator.kt#L27)           |
| `GET`  | [`/subreddits/search`](https://www.reddit.com/dev/api/oauth#GET_subreddits_search)                                 | [`RedditClient.searchSubreddits()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/RedditClient.kt#L299)                            |
| `GET`  | [`/user/{username}/about`](https://www.reddit.com/dev/api/oauth#GET_user_{username}_about)                         | [`UserReference.query()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/UserReference.kt#L39)                           |
| `GET`  | [`/users/{where}`](https://www.reddit.com/dev/api/oauth#GET_users_{where})                                         | [`RedditClient.userSubreddits()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/RedditClient.kt#L282)                              |
| `GET`  | [`[/r/{subreddit}]/{sort}`](https://www.reddit.com/dev/api/oauth#GET_{sort})                                       | [`SubredditReference.posts()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L45)                 |
| `GET`  | [`[/r/{subreddit}]/about/{location}`](https://www.reddit.com/dev/api/oauth#GET_about_{location})                   | None                                                                                                                                                                 |
| `GET`  | [`[/r/{subreddit}]/about/{where}`](https://www.reddit.com/dev/api/oauth#GET_about_{where})                         | None                                                                                                                                                                 |
| `GET`  | [`/api/recommend/sr/{srnames}`](https://www.reddit.com/dev/api/oauth#GET_api_recommend_sr_{srnames})               | None                                                                                                                                                                 |
| `GET`  | [`/api/subreddit_autocomplete`](https://www.reddit.com/dev/api/oauth#GET_api_subreddit_autocomplete)               | None                                                                                                                                                                 |
| `GET`  | [`/api/subreddit_autocomplete_v2`](https://www.reddit.com/dev/api/oauth#GET_api_subreddit_autocomplete_v2)         | None                                                                                                                                                                 |
| `GET`  | [`/by_id/{names}`](https://www.reddit.com/dev/api/oauth#GET_by_id_{names})                                         | None                                                                                                                                                                 |
| `GET`  | [`/duplicates/{article}`](https://www.reddit.com/dev/api/oauth#GET_duplicates_{article})                           | None                                                                                                                                                                 |
| `GET`  | [`/live/{thread}/contributors`](https://www.reddit.com/dev/api/oauth#GET_live_{thread}_contributors)               | None                                                                                                                                                                 |
| `GET`  | [`/live/{thread}/discussions`](https://www.reddit.com/dev/api/oauth#GET_live_{thread}_discussions)                 | None                                                                                                                                                                 |
| `GET`  | [`/live/{thread}/updates/{update_id}`](https://www.reddit.com/dev/api/oauth#GET_live_{thread}_updates_{update_id}) | None                                                                                                                                                                 |
| `GET`  | [`/prefs/{where}`](https://www.reddit.com/dev/api/oauth#GET_prefs_{where})                                         | None                                                                                                                                                                 |
| `GET`  | [`/profiles/search`](https://www.reddit.com/dev/api/oauth#GET_profiles_search)                                     | None                                                                                                                                                                 |
| `GET`  | [`[/r/{subreddit}]/sidebar`](https://www.reddit.com/dev/api/oauth#GET_sidebar)                                     | None                                                                                                                                                                 |
| `GET`  | [`[/r/{subreddit}]/sticky`](https://www.reddit.com/dev/api/oauth#GET_sticky)                                       | None                                                                                                                                                                 |
| `GET`  | [`/subreddits/{where}`](https://www.reddit.com/dev/api/oauth#GET_subreddits_{where})                               | None                                                                                                                                                                 |
| `GET`  | [`/api/live/by_id/{names}`](https://www.reddit.com/dev/api/oauth#GET_api_live_by_id_{names})                       | Not planned                                                                                                                                                          |
| `GET`  | [`/api/search_reddit_names`](https://www.reddit.com/dev/api/oauth#GET_api_search_reddit_names)                     | Not planned                                                                                                                                                          |
| `POST` | [`/api/search_reddit_names`](https://www.reddit.com/dev/api/oauth#POST_api_search_reddit_names)                    | Not planned                                                                                                                                                          |

report
------

66.67% completion (2 implemented, 2 planned, and 1 not planned)

| Method | Endpoint                                                                                          | Implementation                                                                                                                                             |
|:------:| ------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `POST` | [`/api/hide`](https://www.reddit.com/dev/api/oauth#POST_api_hide)                                 | [`SubmissionReference.setHidden()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubmissionReference.kt#L78) |
| `POST` | [`/api/unhide`](https://www.reddit.com/dev/api/oauth#POST_api_unhide)                             | [`SubmissionReference.setHidden()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubmissionReference.kt#L78) |
| `POST` | [`/api/live/{thread}/report`](https://www.reddit.com/dev/api/oauth#POST_api_live_{thread}_report) | None                                                                                                                                                       |
| `POST` | [`/api/report`](https://www.reddit.com/dev/api/oauth#POST_api_report)                             | None                                                                                                                                                       |
| `POST` | [`/api/report_user`](https://www.reddit.com/dev/api/oauth#POST_api_report_user)                   | Not planned                                                                                                                                                |

save
----

100.00% completion (2 implemented, 1 planned, and 1 not planned)

| Method | Endpoint                                                                                 | Implementation                                                                                                                                                            |
|:------:| ---------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `POST` | [`/api/save`](https://www.reddit.com/dev/api/oauth#POST_api_save)                        | [`PublicContributionReference.setSaved()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/PublicContributionReference.kt#L73) |
| `POST` | [`/api/unsave`](https://www.reddit.com/dev/api/oauth#POST_api_unsave)                    | [`PublicContributionReference.setSaved()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/PublicContributionReference.kt#L73) |
| `GET`  | [`/api/saved_categories`](https://www.reddit.com/dev/api/oauth#GET_api_saved_categories) | None                                                                                                                                                                      |
| `POST` | [`/api/store_visits`](https://www.reddit.com/dev/api/oauth#POST_api_store_visits)        | Not planned                                                                                                                                                               |

structuredstyles
----------------

33.33% completion (3 implemented, 6 planned, and 0 not planned)

|  Method  | Endpoint                                                                                                                                    | Implementation                                                                                                                                 |
|:--------:| ------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
|  `POST`  | [`/api/v1/{subreddit}/emoji.json`](https://www.reddit.com/dev/api/oauth#POST_api_v1_{subreddit}_emoji.json)                                 | [`EmojiReference.upload()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/EmojiReference.kt#L43)  |
| `DELETE` | [`/api/v1/{subreddit}/emoji/{emoji_name}`](https://www.reddit.com/dev/api/oauth#DELETE_api_v1_{subreddit}_emoji_{emoji_name})               | [`EmojiReference.delete()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/EmojiReference.kt#L115) |
|  `POST`  | [`/api/v1/{subreddit}/emoji_asset_upload_s3.json`](https://www.reddit.com/dev/api/oauth#POST_api_v1_{subreddit}_emoji_asset_upload_s3.json) | [`EmojiReference.upload()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/EmojiReference.kt#L43)  |
|  `POST`  | [`/api/widget`](https://www.reddit.com/dev/api/oauth#POST_api_widget)                                                                       | None                                                                                                                                           |
| `DELETE` | [`/api/widget/{widget_id}`](https://www.reddit.com/dev/api/oauth#DELETE_api_widget_{widget_id})                                             | None                                                                                                                                           |
|  `PUT`   | [`/api/widget/{widget_id}`](https://www.reddit.com/dev/api/oauth#PUT_api_widget_{widget_id})                                                | None                                                                                                                                           |
|  `POST`  | [`/api/widget_image_upload_s3`](https://www.reddit.com/dev/api/oauth#POST_api_widget_image_upload_s3)                                       | None                                                                                                                                           |
| `PATCH`  | [`/api/widget_order/{section}`](https://www.reddit.com/dev/api/oauth#PATCH_api_widget_order_{section})                                      | None                                                                                                                                           |
|  `GET`   | [`/api/widgets`](https://www.reddit.com/dev/api/oauth#GET_api_widgets)                                                                      | None                                                                                                                                           |

submit
------

100.00% completion (4 implemented, 0 planned, and 0 not planned)

| Method | Endpoint                                                                                          | Implementation                                                                                                                                                 |
|:------:| ------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `POST` | [`/api/live/create`](https://www.reddit.com/dev/api/oauth#POST_api_live_create)                   | [`SelfUserReference.createLiveThread()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SelfUserReference.kt#L170) |
| `POST` | [`/api/live/{thread}/update`](https://www.reddit.com/dev/api/oauth#POST_api_live_{thread}_update) | [`LiveThreadReference.postUpdate()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/LiveThreadReference.kt#L62)    |
| `POST` | [`/api/submit`](https://www.reddit.com/dev/api/oauth#POST_api_submit)                             | [`SubredditReference.submit()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L93)          |
| `GET`  | [`[/r/{subreddit}]/api/submit_text`](https://www.reddit.com/dev/api/oauth#GET_api_submit_text)    | [`SubredditReference.submitText()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L121)     |

subscribe
---------

80.00% completion (8 implemented, 2 planned, and 0 not planned)

|  Method  | Endpoint                                                                                                            | Implementation                                                                                                                                                      |
|:--------:| ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|  `POST`  | [`/api/multi/copy`](https://www.reddit.com/dev/api/oauth#POST_api_multi_copy)                                       | [`MultiredditReference.copyTo()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/MultiredditReference.kt#L88)           |
|  `POST`  | [`/api/multi/rename`](https://www.reddit.com/dev/api/oauth#POST_api_multi_rename)                                   | [`MultiredditReference.rename()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/MultiredditReference.kt#L96)           |
| `DELETE` | [`/api/multi/{multipath}`](https://www.reddit.com/dev/api/oauth#DELETE_api_multi_{multipath})                       | [`MultiredditReference.delete()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/MultiredditReference.kt#L76)           |
|  `POST`  | [`/api/multi/{multipath}`](https://www.reddit.com/dev/api/oauth#POST_api_multi_{multipath})                         | [`MultiredditReference.createOrUpdate()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/MultiredditReference.kt#L36)   |
|  `PUT`   | [`/api/multi/{multipath}`](https://www.reddit.com/dev/api/oauth#PUT_api_multi_{multipath})                          | [`MultiredditReference.createOrUpdate()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/MultiredditReference.kt#L36)   |
| `DELETE` | [`/api/multi/{multipath}/r/{srname}`](https://www.reddit.com/dev/api/oauth#DELETE_api_multi_{multipath}_r_{srname}) | [`MultiredditReference.removeSubreddit()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/MultiredditReference.kt#L142) |
|  `PUT`   | [`/api/multi/{multipath}/r/{srname}`](https://www.reddit.com/dev/api/oauth#PUT_api_multi_{multipath}_r_{srname})    | [`MultiredditReference.addSubreddit()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/MultiredditReference.kt#L130)    |
|  `POST`  | [`/api/subscribe`](https://www.reddit.com/dev/api/oauth#POST_api_subscribe)                                         | [`SubredditReference.setSubscribed()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/SubredditReference.kt#L137)       |
| `DELETE` | [`/api/v1/me/friends/{username}`](https://www.reddit.com/dev/api/oauth#DELETE_api_v1_me_friends_{username})         | None                                                                                                                                                                |
|  `PUT`   | [`/api/v1/me/friends/{username}`](https://www.reddit.com/dev/api/oauth#PUT_api_v1_me_friends_{username})            | None                                                                                                                                                                |

vote
----

100.00% completion (1 implemented, 0 planned, and 0 not planned)

| Method | Endpoint                                                          | Implementation                                                                                                                                                           |
|:------:| ----------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `POST` | [`/api/vote`](https://www.reddit.com/dev/api/oauth#POST_api_vote) | [`PublicContributionReference.setVote()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/PublicContributionReference.kt#L47) |

wikiedit
--------

100.00% completion (1 implemented, 0 planned, and 0 not planned)

| Method | Endpoint                                                                                    | Implementation                                                                                                                              |
|:------:| ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| `POST` | [`[/r/{subreddit}]/api/wiki/edit`](https://www.reddit.com/dev/api/oauth#POST_api_wiki_edit) | [`WikiReference.update()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/WikiReference.kt#L36) |

wikiread
--------

100.00% completion (5 implemented, 0 planned, and 0 not planned)

| Method | Endpoint                                                                                                       | Implementation                                                                                                                                        |
|:------:| -------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| `GET`  | [`[/r/{subreddit}]/wiki/discussions/{page}`](https://www.reddit.com/dev/api/oauth#GET_wiki_discussions_{page}) | [`WikiReference.discussionsAbout()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/WikiReference.kt#L59) |
| `GET`  | [`[/r/{subreddit}]/wiki/pages`](https://www.reddit.com/dev/api/oauth#GET_wiki_pages)                           | [`WikiReference.pages()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/WikiReference.kt#L20)            |
| `GET`  | [`[/r/{subreddit}]/wiki/revisions`](https://www.reddit.com/dev/api/oauth#GET_wiki_revisions)                   | [`WikiReference.revisions()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/WikiReference.kt#L49)        |
| `GET`  | [`[/r/{subreddit}]/wiki/revisions/{page}`](https://www.reddit.com/dev/api/oauth#GET_wiki_revisions_{page})     | [`WikiReference.revisionsFor()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/WikiReference.kt#L54)     |
| `GET`  | [`[/r/{subreddit}]/wiki/{page}`](https://www.reddit.com/dev/api/oauth#GET_wiki_{page})                         | [`WikiReference.page()`](https://github.com/mattbdean/JRAW/tree/master/lib/src/main/kotlin/net/dean/jraw/references/WikiReference.kt#L28)             |

