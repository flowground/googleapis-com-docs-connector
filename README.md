# ![LOGO](logo.png) Google Docs **flow**ground Connector

## Description

A generated **flow**ground connector for the Google Docs API (version v1).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/docs/v1/swagger.json<br/>
Generated at: 2019-05-07T17:41:36+03:00

## API Description

Reads and writes Google Docs documents.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Creates a blank document using the title given in the request. Other fields<br/>
> in the request, including any provided content, are ignored.<br/>
> <br/>
> Returns the created document.

*Tags:* `documents`

#### Input Parameters
* `$.xgafv` - _optional_ - V1 error format.
    Possible values: 1, 2.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Gets the latest version of the specified document.

*Tags:* `documents`

#### Input Parameters
* `documentId` - _required_ - The ID of the document to retrieve.
* `suggestionsViewMode` - _optional_ - The suggestions view mode to apply to the document. This allows viewing the
document with all suggestions inline, accepted or rejected. If one is not
specified, DEFAULT_FOR_CURRENT_ACCESS is
used.
    Possible values: DEFAULT_FOR_CURRENT_ACCESS, SUGGESTIONS_INLINE, PREVIEW_SUGGESTIONS_ACCEPTED, PREVIEW_WITHOUT_SUGGESTIONS.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Applies one or more updates to the document.<br/>
> <br/>
> Each request is validated before<br/>
> being applied. If any request is not valid, then the entire request will<br/>
> fail and nothing will be applied.<br/>
> <br/>
> Some requests have replies to<br/>
> give you some information about how they are applied. Other requests do<br/>
> not need to return information; these each return an empty reply.<br/>
> The order of replies matches that of the requests.<br/>
> <br/>
> For example, suppose you call batchUpdate with four updates, and only the<br/>
> third one returns information. The response would have two empty replies,<br/>
> the reply to the third request, and another empty reply, in that order.<br/>
> <br/>
> Because other users may be editing the document, the document<br/>
> might not exactly reflect your changes: your changes may<br/>
> be altered with respect to collaborator changes. If there are no<br/>
> collaborators, the document should reflect your changes. In any case,<br/>
> the updates in your request are guaranteed to be applied together<br/>
> atomically.

*Tags:* `documents`

#### Input Parameters
* `documentId` - _required_ - The ID of the document to update.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

## License

**flow**ground :- Telekom iPaaS / googleapis-com-docs-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
