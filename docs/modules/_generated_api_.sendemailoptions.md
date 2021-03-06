# Module: SendEmailOptions

**`export`** 

**`namespace`** SendEmailOptions

## Properties

### `Optional` attachments

• **attachments**? : *Array‹string›*

*Defined in [src/generated/api.ts:1979](https://github.com/mailslurp/mailslurp-client-ts-js/blob/507ad2d/src/generated/api.ts#L1979)*

Optional list of attachment IDs to send with this email. You must first upload each attachment separately in order to obtain attachment IDs. This way you can reuse attachments with different emails once uploaded.

**`type`** {Array<string>}

**`memberof`** SendEmailOptions

___

### `Optional` bcc

• **bcc**? : *Array‹string›*

*Defined in [src/generated/api.ts:1985](https://github.com/mailslurp/mailslurp-client-ts-js/blob/507ad2d/src/generated/api.ts#L1985)*

Optional list of bcc destination email addresses

**`type`** {Array<string>}

**`memberof`** SendEmailOptions

___

### `Optional` body

• **body**? : *string*

*Defined in [src/generated/api.ts:1991](https://github.com/mailslurp/mailslurp-client-ts-js/blob/507ad2d/src/generated/api.ts#L1991)*

Optional contents of email. If body contains HTML then set `isHTML` to true to ensure that email clients render it correctly. You can use moustache template syntax in the email body in conjunction with `toGroup` contact variables or `templateVariables` data. If you need more templating control consider creating a template and using the `template` property instead of the body.

**`type`** {string}

**`memberof`** SendEmailOptions

___

### `Optional` cc

• **cc**? : *Array‹string›*

*Defined in [src/generated/api.ts:1997](https://github.com/mailslurp/mailslurp-client-ts-js/blob/507ad2d/src/generated/api.ts#L1997)*

Optional list of cc destination email addresses

**`type`** {Array<string>}

**`memberof`** SendEmailOptions

___

### `Optional` charset

• **charset**? : *string*

*Defined in [src/generated/api.ts:2003](https://github.com/mailslurp/mailslurp-client-ts-js/blob/507ad2d/src/generated/api.ts#L2003)*

Optional charset

**`type`** {string}

**`memberof`** SendEmailOptions

___

### `Optional` from

• **from**? : *string*

*Defined in [src/generated/api.ts:2009](https://github.com/mailslurp/mailslurp-client-ts-js/blob/507ad2d/src/generated/api.ts#L2009)*

Optional from address. If not set the source inbox address will be used for this field. Beware of potential spam penalties when setting this field to an address not used by the inbox. For custom email addresses use a custom domain.

**`type`** {string}

**`memberof`** SendEmailOptions

___

### `Optional` isHTML

• **isHTML**? : *boolean*

*Defined in [src/generated/api.ts:2015](https://github.com/mailslurp/mailslurp-client-ts-js/blob/507ad2d/src/generated/api.ts#L2015)*

Optional HTML flag. If true the `content-type` of the email will be `text/html`. Set to true when sending HTML to ensure proper rending on email clients

**`type`** {boolean}

**`memberof`** SendEmailOptions

___

### `Optional` replyTo

• **replyTo**? : *string*

*Defined in [src/generated/api.ts:2021](https://github.com/mailslurp/mailslurp-client-ts-js/blob/507ad2d/src/generated/api.ts#L2021)*

Optional replyTo header

**`type`** {string}

**`memberof`** SendEmailOptions

___

### `Optional` sendStrategy

• **sendStrategy**? : *[SendStrategyEnum](../enums/_generated_api_.sendemailoptions.sendstrategyenum.md)*

*Defined in [src/generated/api.ts:2027](https://github.com/mailslurp/mailslurp-client-ts-js/blob/507ad2d/src/generated/api.ts#L2027)*

Optional strategy to use when sending the email

**`type`** {string}

**`memberof`** SendEmailOptions

___

### `Optional` subject

• **subject**? : *string*

*Defined in [src/generated/api.ts:2033](https://github.com/mailslurp/mailslurp-client-ts-js/blob/507ad2d/src/generated/api.ts#L2033)*

Optional email subject line

**`type`** {string}

**`memberof`** SendEmailOptions

___

### `Optional` template

• **template**? : *string*

*Defined in [src/generated/api.ts:2039](https://github.com/mailslurp/mailslurp-client-ts-js/blob/507ad2d/src/generated/api.ts#L2039)*

Optional template ID to use for body. Will override body if provided. When using a template make sure you pass the corresponding map of `templateVariables`. You can find which variables are needed by fetching the template itself or viewing it in the dashboard.

**`type`** {string}

**`memberof`** SendEmailOptions

___

### `Optional` templateVariables

• **templateVariables**? : *any*

*Defined in [src/generated/api.ts:2045](https://github.com/mailslurp/mailslurp-client-ts-js/blob/507ad2d/src/generated/api.ts#L2045)*

Optional map of template variables. Will replace moustache syntax variables in subject and body or template with the associated values if found.

**`type`** {any}

**`memberof`** SendEmailOptions

___

### `Optional` to

• **to**? : *Array‹string›*

*Defined in [src/generated/api.ts:2051](https://github.com/mailslurp/mailslurp-client-ts-js/blob/507ad2d/src/generated/api.ts#L2051)*

List of destination email addresses. Even single recipients must be in array form. Maximum recipients per email depends on your plan. If you need to send many emails try using contacts or contact groups or use a non standard sendStrategy to ensure that spam filters are not triggered (many recipients in one email can affect your spam rating).

**`type`** {Array<string>}

**`memberof`** SendEmailOptions

___

### `Optional` toContacts

• **toContacts**? : *Array‹string›*

*Defined in [src/generated/api.ts:2057](https://github.com/mailslurp/mailslurp-client-ts-js/blob/507ad2d/src/generated/api.ts#L2057)*

Optional list of contact IDs to send email to. Manage your contacts via the API or dashboard. When contacts are used the email is sent to each contact separately so they will not see other recipients.

**`type`** {Array<string>}

**`memberof`** SendEmailOptions

___

### `Optional` toGroup

• **toGroup**? : *string*

*Defined in [src/generated/api.ts:2063](https://github.com/mailslurp/mailslurp-client-ts-js/blob/507ad2d/src/generated/api.ts#L2063)*

Optional contact group ID to send email to. You can create contacts and contact groups in the API or dashboard and use them for email campaigns. When contact groups are used the email is sent to each contact separately so they will not see other recipients

**`type`** {string}

**`memberof`** SendEmailOptions
