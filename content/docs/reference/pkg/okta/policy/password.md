
---
title: "Password"
block_external_search_index: true
---



Creates a Password Policy.

This resource allows you to create and configure a Password Policy.

## Example Usage

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as okta from "@pulumi/okta";

const example = new okta.policy.Password("example", {
    description: "Example",
    groupsIncludeds: [okta_group_everyone.id],
    passwordHistoryCount: 4,
    status: "ACTIVE",
});
```

> This content is derived from https://github.com/articulate/terraform-provider-okta/blob/master/website/docs/r/policy_password.html.markdown.



## Create a Password Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/okta/policy/#Password">Password</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/okta/policy/#PasswordArgs">PasswordArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">pulumi.CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">Password</span><span class="p">(resource_name, opts=None, </span>auth_provider=None<span class="p">, </span>description=None<span class="p">, </span>email_recovery=None<span class="p">, </span>groups_includeds=None<span class="p">, </span>name=None<span class="p">, </span>password_auto_unlock_minutes=None<span class="p">, </span>password_dictionary_lookup=None<span class="p">, </span>password_exclude_first_name=None<span class="p">, </span>password_exclude_last_name=None<span class="p">, </span>password_exclude_username=None<span class="p">, </span>password_expire_warn_days=None<span class="p">, </span>password_history_count=None<span class="p">, </span>password_max_age_days=None<span class="p">, </span>password_max_lockout_attempts=None<span class="p">, </span>password_min_age_minutes=None<span class="p">, </span>password_min_length=None<span class="p">, </span>password_min_lowercase=None<span class="p">, </span>password_min_number=None<span class="p">, </span>password_min_symbol=None<span class="p">, </span>password_min_uppercase=None<span class="p">, </span>password_show_lockout_failures=None<span class="p">, </span>priority=None<span class="p">, </span>question_min_length=None<span class="p">, </span>question_recovery=None<span class="p">, </span>recovery_email_token=None<span class="p">, </span>skip_unlock=None<span class="p">, </span>sms_recovery=None<span class="p">, </span>status=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewPassword<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">pulumi.Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#PasswordArgs">PasswordArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">pulumi.ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#Password">Password</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Okta/Pulumi.Okta.Policy.Password.html">Password</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Okta/Pulumi.Okta.Policy.PasswordArgs.html">PasswordArgs</a></span>? <span class="nx">args = null<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

#### Resource Arguments




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Auth<wbr>Provider</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Authentication Provider: `"OKTA"` or `"ACTIVE_DIRECTORY"`. Default is `"OKTA"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Description.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Email<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable email password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Groups<wbr>Includeds</span>
        <span class="property-indicator"></span>
        <span class="property-type">List<string>?</span>
    </dt>
    <dd>{{% md %}}List of Group IDs to Include.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Auto<wbr>Unlock<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Number of minutes before a locked account is unlocked: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Dictionary<wbr>Lookup</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Check Passwords Against Common Password Dictionary.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Exclude<wbr>First<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}User firstName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Exclude<wbr>Last<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}User lastName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Exclude<wbr>Username</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}If the user name must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Expire<wbr>Warn<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Length in days a user will be warned before password expiry: 0 = no warning.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>History<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Number of distinct passwords that must be created before they can be reused: 0 = none.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Max<wbr>Age<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Length in days a password is valid before expiry: 0 = no limit.",
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Max<wbr>Lockout<wbr>Attempts</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Number of unsuccessful login attempts allowed before lockout: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Age<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum time interval in minutes between password changes: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum password length. Default is 8.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Lowercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum number of lower case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum number of numbers in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Symbol</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum number of symbols in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Uppercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum number of upper case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Show<wbr>Lockout<wbr>Failures</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}If a user should be informed when their account is locked.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Priority of the policy.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Question<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Min length of the password recovery question answer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Question<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable security question password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Recovery<wbr>Email<wbr>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Lifetime in minutes of the recovery email token.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Skip<wbr>Unlock</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}When an Active Directory user is locked out of Okta, the Okta unlock operation should also attempt to unlock the user's Windows account.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Sms<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable SMS password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Auth<wbr>Provider</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Authentication Provider: `"OKTA"` or `"ACTIVE_DIRECTORY"`. Default is `"OKTA"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy Description.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Email<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Enable or disable email password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Groups<wbr>Includeds</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}List of Group IDs to Include.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Auto<wbr>Unlock<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Number of minutes before a locked account is unlocked: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Dictionary<wbr>Lookup</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Check Passwords Against Common Password Dictionary.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Exclude<wbr>First<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}User firstName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Exclude<wbr>Last<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}User lastName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Exclude<wbr>Username</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}If the user name must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Expire<wbr>Warn<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Length in days a user will be warned before password expiry: 0 = no warning.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>History<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Number of distinct passwords that must be created before they can be reused: 0 = none.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Max<wbr>Age<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Length in days a password is valid before expiry: 0 = no limit.",
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Max<wbr>Lockout<wbr>Attempts</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Number of unsuccessful login attempts allowed before lockout: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Age<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum time interval in minutes between password changes: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum password length. Default is 8.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Lowercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum number of lower case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum number of numbers in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Symbol</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum number of symbols in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Uppercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum number of upper case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Show<wbr>Lockout<wbr>Failures</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}If a user should be informed when their account is locked.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Priority of the policy.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Question<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Min length of the password recovery question answer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Question<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Enable or disable security question password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Recovery<wbr>Email<wbr>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Lifetime in minutes of the recovery email token.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Skip<wbr>Unlock</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}When an Active Directory user is locked out of Okta, the Okta unlock operation should also attempt to unlock the user's Windows account.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Sms<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Enable or disable SMS password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>auth<wbr>Provider</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Authentication Provider: `"OKTA"` or `"ACTIVE_DIRECTORY"`. Default is `"OKTA"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Description.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>email<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable email password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>groups<wbr>Includeds</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]?</span>
    </dt>
    <dd>{{% md %}}List of Group IDs to Include.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Auto<wbr>Unlock<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Number of minutes before a locked account is unlocked: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Dictionary<wbr>Lookup</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Check Passwords Against Common Password Dictionary.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Exclude<wbr>First<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}User firstName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Exclude<wbr>Last<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}User lastName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Exclude<wbr>Username</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}If the user name must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Expire<wbr>Warn<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Length in days a user will be warned before password expiry: 0 = no warning.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>History<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Number of distinct passwords that must be created before they can be reused: 0 = none.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Max<wbr>Age<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Length in days a password is valid before expiry: 0 = no limit.",
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Max<wbr>Lockout<wbr>Attempts</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Number of unsuccessful login attempts allowed before lockout: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Min<wbr>Age<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum time interval in minutes between password changes: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum password length. Default is 8.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Min<wbr>Lowercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum number of lower case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Min<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum number of numbers in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Min<wbr>Symbol</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum number of symbols in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Min<wbr>Uppercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum number of upper case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Show<wbr>Lockout<wbr>Failures</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}If a user should be informed when their account is locked.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Priority of the policy.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>question<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Min length of the password recovery question answer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>question<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable security question password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>recovery<wbr>Email<wbr>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Lifetime in minutes of the recovery email token.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>skip<wbr>Unlock</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}When an Active Directory user is locked out of Okta, the Okta unlock operation should also attempt to unlock the user's Windows account.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>sms<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable SMS password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>auth_<wbr>provider</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Authentication Provider: `"OKTA"` or `"ACTIVE_DIRECTORY"`. Default is `"OKTA"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Description.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>email_<wbr>recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Enable or disable email password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>groups_<wbr>includeds</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}List of Group IDs to Include.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>auto_<wbr>unlock_<wbr>minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of minutes before a locked account is unlocked: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>dictionary_<wbr>lookup</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Check Passwords Against Common Password Dictionary.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>exclude_<wbr>first_<wbr>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}User firstName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>exclude_<wbr>last_<wbr>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}User lastName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>exclude_<wbr>username</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}If the user name must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>expire_<wbr>warn_<wbr>days</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Length in days a user will be warned before password expiry: 0 = no warning.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>history_<wbr>count</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of distinct passwords that must be created before they can be reused: 0 = none.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>max_<wbr>age_<wbr>days</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Length in days a password is valid before expiry: 0 = no limit.",
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>max_<wbr>lockout_<wbr>attempts</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of unsuccessful login attempts allowed before lockout: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>min_<wbr>age_<wbr>minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum time interval in minutes between password changes: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>min_<wbr>length</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum password length. Default is 8.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>min_<wbr>lowercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum number of lower case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>min_<wbr>number</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum number of numbers in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>min_<wbr>symbol</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum number of symbols in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>min_<wbr>uppercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum number of upper case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>show_<wbr>lockout_<wbr>failures</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}If a user should be informed when their account is locked.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Priority of the policy.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>question_<wbr>min_<wbr>length</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Min length of the password recovery question answer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>question_<wbr>recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Enable or disable security question password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>recovery_<wbr>email_<wbr>token</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Lifetime in minutes of the recovery email token.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>skip_<wbr>unlock</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}When an Active Directory user is locked out of Okta, the Okta unlock operation should also attempt to unlock the user's Windows account.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>sms_<wbr>recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Enable or disable SMS password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}







## Password Output Properties

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Auth<wbr>Provider</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Authentication Provider: `"OKTA"` or `"ACTIVE_DIRECTORY"`. Default is `"OKTA"`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Description.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Email<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable email password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Groups<wbr>Includeds</span>
        <span class="property-indicator"></span>
        <span class="property-type">List<string>?</span>
    </dt>
    <dd>{{% md %}}List of Group IDs to Include.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Policy Name.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Auto<wbr>Unlock<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Number of minutes before a locked account is unlocked: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Dictionary<wbr>Lookup</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Check Passwords Against Common Password Dictionary.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Exclude<wbr>First<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}User firstName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Exclude<wbr>Last<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}User lastName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Exclude<wbr>Username</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}If the user name must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Expire<wbr>Warn<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Length in days a user will be warned before password expiry: 0 = no warning.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>History<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Number of distinct passwords that must be created before they can be reused: 0 = none.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Max<wbr>Age<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Length in days a password is valid before expiry: 0 = no limit.",
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Max<wbr>Lockout<wbr>Attempts</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Number of unsuccessful login attempts allowed before lockout: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Min<wbr>Age<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum time interval in minutes between password changes: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum password length. Default is 8.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Min<wbr>Lowercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum number of lower case characters in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Min<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum number of numbers in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Min<wbr>Symbol</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum number of symbols in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Min<wbr>Uppercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum number of upper case characters in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Show<wbr>Lockout<wbr>Failures</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}If a user should be informed when their account is locked.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Priority of the policy.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Question<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Min length of the password recovery question answer.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Question<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable security question password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Recovery<wbr>Email<wbr>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Lifetime in minutes of the recovery email token.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Skip<wbr>Unlock</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}When an Active Directory user is locked out of Okta, the Okta unlock operation should also attempt to unlock the user's Windows account.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Sms<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable SMS password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Auth<wbr>Provider</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Authentication Provider: `"OKTA"` or `"ACTIVE_DIRECTORY"`. Default is `"OKTA"`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy Description.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Email<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Enable or disable email password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Groups<wbr>Includeds</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}List of Group IDs to Include.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Policy Name.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Auto<wbr>Unlock<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Number of minutes before a locked account is unlocked: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Dictionary<wbr>Lookup</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Check Passwords Against Common Password Dictionary.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Exclude<wbr>First<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}User firstName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Exclude<wbr>Last<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}User lastName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Exclude<wbr>Username</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}If the user name must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Expire<wbr>Warn<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Length in days a user will be warned before password expiry: 0 = no warning.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>History<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Number of distinct passwords that must be created before they can be reused: 0 = none.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Max<wbr>Age<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Length in days a password is valid before expiry: 0 = no limit.",
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Max<wbr>Lockout<wbr>Attempts</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Number of unsuccessful login attempts allowed before lockout: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Min<wbr>Age<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum time interval in minutes between password changes: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum password length. Default is 8.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Min<wbr>Lowercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum number of lower case characters in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Min<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum number of numbers in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Min<wbr>Symbol</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum number of symbols in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Min<wbr>Uppercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum number of upper case characters in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Password<wbr>Show<wbr>Lockout<wbr>Failures</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}If a user should be informed when their account is locked.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Priority of the policy.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Question<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Min length of the password recovery question answer.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Question<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Enable or disable security question password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Recovery<wbr>Email<wbr>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Lifetime in minutes of the recovery email token.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Skip<wbr>Unlock</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}When an Active Directory user is locked out of Okta, the Okta unlock operation should also attempt to unlock the user's Windows account.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Sms<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Enable or disable SMS password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>auth<wbr>Provider</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Authentication Provider: `"OKTA"` or `"ACTIVE_DIRECTORY"`. Default is `"OKTA"`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Description.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>email<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable email password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>groups<wbr>Includeds</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]?</span>
    </dt>
    <dd>{{% md %}}List of Group IDs to Include.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Policy Name.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>Auto<wbr>Unlock<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Number of minutes before a locked account is unlocked: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>Dictionary<wbr>Lookup</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Check Passwords Against Common Password Dictionary.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>Exclude<wbr>First<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}User firstName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>Exclude<wbr>Last<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}User lastName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>Exclude<wbr>Username</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}If the user name must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>Expire<wbr>Warn<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Length in days a user will be warned before password expiry: 0 = no warning.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>History<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Number of distinct passwords that must be created before they can be reused: 0 = none.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>Max<wbr>Age<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Length in days a password is valid before expiry: 0 = no limit.",
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>Max<wbr>Lockout<wbr>Attempts</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Number of unsuccessful login attempts allowed before lockout: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>Min<wbr>Age<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum time interval in minutes between password changes: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum password length. Default is 8.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>Min<wbr>Lowercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum number of lower case characters in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>Min<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum number of numbers in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>Min<wbr>Symbol</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum number of symbols in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>Min<wbr>Uppercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum number of upper case characters in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password<wbr>Show<wbr>Lockout<wbr>Failures</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}If a user should be informed when their account is locked.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Priority of the policy.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>question<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Min length of the password recovery question answer.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>question<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable security question password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>recovery<wbr>Email<wbr>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Lifetime in minutes of the recovery email token.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>skip<wbr>Unlock</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}When an Active Directory user is locked out of Okta, the Okta unlock operation should also attempt to unlock the user's Windows account.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>sms<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable SMS password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>auth_<wbr>provider</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Authentication Provider: `"OKTA"` or `"ACTIVE_DIRECTORY"`. Default is `"OKTA"`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Description.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>email_<wbr>recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Enable or disable email password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>groups_<wbr>includeds</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}List of Group IDs to Include.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Name.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>auto_<wbr>unlock_<wbr>minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of minutes before a locked account is unlocked: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>dictionary_<wbr>lookup</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Check Passwords Against Common Password Dictionary.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>exclude_<wbr>first_<wbr>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}User firstName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>exclude_<wbr>last_<wbr>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}User lastName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>exclude_<wbr>username</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}If the user name must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>expire_<wbr>warn_<wbr>days</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Length in days a user will be warned before password expiry: 0 = no warning.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>history_<wbr>count</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of distinct passwords that must be created before they can be reused: 0 = none.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>max_<wbr>age_<wbr>days</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Length in days a password is valid before expiry: 0 = no limit.",
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>max_<wbr>lockout_<wbr>attempts</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of unsuccessful login attempts allowed before lockout: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>min_<wbr>age_<wbr>minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum time interval in minutes between password changes: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>min_<wbr>length</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum password length. Default is 8.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>min_<wbr>lowercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum number of lower case characters in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>min_<wbr>number</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum number of numbers in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>min_<wbr>symbol</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum number of symbols in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>min_<wbr>uppercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum number of upper case characters in password.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>password_<wbr>show_<wbr>lockout_<wbr>failures</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}If a user should be informed when their account is locked.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Priority of the policy.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>question_<wbr>min_<wbr>length</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Min length of the password recovery question answer.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>question_<wbr>recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Enable or disable security question password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>recovery_<wbr>email_<wbr>token</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Lifetime in minutes of the recovery email token.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>skip_<wbr>unlock</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}When an Active Directory user is locked out of Okta, the Okta unlock operation should also attempt to unlock the user's Windows account.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>sms_<wbr>recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Enable or disable SMS password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Look up an Existing Password Resource

Get an existing Password resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/okta/policy/#PasswordState">PasswordState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/okta/policy/#Password">Password</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>auth_provider=None<span class="p">, </span>description=None<span class="p">, </span>email_recovery=None<span class="p">, </span>groups_includeds=None<span class="p">, </span>name=None<span class="p">, </span>password_auto_unlock_minutes=None<span class="p">, </span>password_dictionary_lookup=None<span class="p">, </span>password_exclude_first_name=None<span class="p">, </span>password_exclude_last_name=None<span class="p">, </span>password_exclude_username=None<span class="p">, </span>password_expire_warn_days=None<span class="p">, </span>password_history_count=None<span class="p">, </span>password_max_age_days=None<span class="p">, </span>password_max_lockout_attempts=None<span class="p">, </span>password_min_age_minutes=None<span class="p">, </span>password_min_length=None<span class="p">, </span>password_min_lowercase=None<span class="p">, </span>password_min_number=None<span class="p">, </span>password_min_symbol=None<span class="p">, </span>password_min_uppercase=None<span class="p">, </span>password_show_lockout_failures=None<span class="p">, </span>priority=None<span class="p">, </span>question_min_length=None<span class="p">, </span>question_recovery=None<span class="p">, </span>recovery_email_token=None<span class="p">, </span>skip_unlock=None<span class="p">, </span>sms_recovery=None<span class="p">, </span>status=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetPassword<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#PasswordState">PasswordState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#Password">Password</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Okta/Pulumi.Okta.Policy.Password.html">Password</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Okta/Pulumi.Okta.Policy.PasswordState.html">PasswordState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>resource_name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Optional">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

The following state arguments are supported:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Auth<wbr>Provider</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Authentication Provider: `"OKTA"` or `"ACTIVE_DIRECTORY"`. Default is `"OKTA"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Description.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Email<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable email password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Groups<wbr>Includeds</span>
        <span class="property-indicator"></span>
        <span class="property-type">List<string>?</span>
    </dt>
    <dd>{{% md %}}List of Group IDs to Include.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Auto<wbr>Unlock<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Number of minutes before a locked account is unlocked: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Dictionary<wbr>Lookup</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Check Passwords Against Common Password Dictionary.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Exclude<wbr>First<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}User firstName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Exclude<wbr>Last<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}User lastName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Exclude<wbr>Username</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}If the user name must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Expire<wbr>Warn<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Length in days a user will be warned before password expiry: 0 = no warning.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>History<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Number of distinct passwords that must be created before they can be reused: 0 = none.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Max<wbr>Age<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Length in days a password is valid before expiry: 0 = no limit.",
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Max<wbr>Lockout<wbr>Attempts</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Number of unsuccessful login attempts allowed before lockout: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Age<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum time interval in minutes between password changes: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum password length. Default is 8.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Lowercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum number of lower case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum number of numbers in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Symbol</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum number of symbols in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Uppercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Minimum number of upper case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Show<wbr>Lockout<wbr>Failures</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}If a user should be informed when their account is locked.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Priority of the policy.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Question<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Min length of the password recovery question answer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Question<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable security question password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Recovery<wbr>Email<wbr>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Lifetime in minutes of the recovery email token.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Skip<wbr>Unlock</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}When an Active Directory user is locked out of Okta, the Okta unlock operation should also attempt to unlock the user's Windows account.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Sms<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable SMS password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Auth<wbr>Provider</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Authentication Provider: `"OKTA"` or `"ACTIVE_DIRECTORY"`. Default is `"OKTA"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy Description.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Email<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Enable or disable email password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Groups<wbr>Includeds</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}List of Group IDs to Include.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Auto<wbr>Unlock<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Number of minutes before a locked account is unlocked: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Dictionary<wbr>Lookup</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Check Passwords Against Common Password Dictionary.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Exclude<wbr>First<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}User firstName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Exclude<wbr>Last<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}User lastName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Exclude<wbr>Username</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}If the user name must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Expire<wbr>Warn<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Length in days a user will be warned before password expiry: 0 = no warning.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>History<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Number of distinct passwords that must be created before they can be reused: 0 = none.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Max<wbr>Age<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Length in days a password is valid before expiry: 0 = no limit.",
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Max<wbr>Lockout<wbr>Attempts</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Number of unsuccessful login attempts allowed before lockout: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Age<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum time interval in minutes between password changes: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum password length. Default is 8.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Lowercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum number of lower case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum number of numbers in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Symbol</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum number of symbols in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Min<wbr>Uppercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Minimum number of upper case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password<wbr>Show<wbr>Lockout<wbr>Failures</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}If a user should be informed when their account is locked.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Priority of the policy.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Question<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Min length of the password recovery question answer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Question<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Enable or disable security question password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Recovery<wbr>Email<wbr>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Lifetime in minutes of the recovery email token.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Skip<wbr>Unlock</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}When an Active Directory user is locked out of Okta, the Okta unlock operation should also attempt to unlock the user's Windows account.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Sms<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Enable or disable SMS password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>auth<wbr>Provider</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Authentication Provider: `"OKTA"` or `"ACTIVE_DIRECTORY"`. Default is `"OKTA"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Description.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>email<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable email password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>groups<wbr>Includeds</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]?</span>
    </dt>
    <dd>{{% md %}}List of Group IDs to Include.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Auto<wbr>Unlock<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Number of minutes before a locked account is unlocked: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Dictionary<wbr>Lookup</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Check Passwords Against Common Password Dictionary.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Exclude<wbr>First<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}User firstName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Exclude<wbr>Last<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}User lastName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Exclude<wbr>Username</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}If the user name must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Expire<wbr>Warn<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Length in days a user will be warned before password expiry: 0 = no warning.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>History<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Number of distinct passwords that must be created before they can be reused: 0 = none.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Max<wbr>Age<wbr>Days</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Length in days a password is valid before expiry: 0 = no limit.",
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Max<wbr>Lockout<wbr>Attempts</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Number of unsuccessful login attempts allowed before lockout: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Min<wbr>Age<wbr>Minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum time interval in minutes between password changes: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum password length. Default is 8.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Min<wbr>Lowercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum number of lower case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Min<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum number of numbers in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Min<wbr>Symbol</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum number of symbols in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Min<wbr>Uppercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Minimum number of upper case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password<wbr>Show<wbr>Lockout<wbr>Failures</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}If a user should be informed when their account is locked.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Priority of the policy.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>question<wbr>Min<wbr>Length</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Min length of the password recovery question answer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>question<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable security question password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>recovery<wbr>Email<wbr>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Lifetime in minutes of the recovery email token.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>skip<wbr>Unlock</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}When an Active Directory user is locked out of Okta, the Okta unlock operation should also attempt to unlock the user's Windows account.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>sms<wbr>Recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Enable or disable SMS password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>auth_<wbr>provider</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Authentication Provider: `"OKTA"` or `"ACTIVE_DIRECTORY"`. Default is `"OKTA"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Description.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>email_<wbr>recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Enable or disable email password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>groups_<wbr>includeds</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}List of Group IDs to Include.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>auto_<wbr>unlock_<wbr>minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of minutes before a locked account is unlocked: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>dictionary_<wbr>lookup</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Check Passwords Against Common Password Dictionary.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>exclude_<wbr>first_<wbr>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}User firstName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>exclude_<wbr>last_<wbr>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}User lastName attribute must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>exclude_<wbr>username</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}If the user name must be excluded from the password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>expire_<wbr>warn_<wbr>days</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Length in days a user will be warned before password expiry: 0 = no warning.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>history_<wbr>count</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of distinct passwords that must be created before they can be reused: 0 = none.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>max_<wbr>age_<wbr>days</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Length in days a password is valid before expiry: 0 = no limit.",
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>max_<wbr>lockout_<wbr>attempts</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of unsuccessful login attempts allowed before lockout: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>min_<wbr>age_<wbr>minutes</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum time interval in minutes between password changes: 0 = no limit.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>min_<wbr>length</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum password length. Default is 8.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>min_<wbr>lowercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum number of lower case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>min_<wbr>number</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum number of numbers in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>min_<wbr>symbol</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum number of symbols in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>min_<wbr>uppercase</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Minimum number of upper case characters in password.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password_<wbr>show_<wbr>lockout_<wbr>failures</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}If a user should be informed when their account is locked.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Priority of the policy.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>question_<wbr>min_<wbr>length</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Min length of the password recovery question answer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>question_<wbr>recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Enable or disable security question password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>recovery_<wbr>email_<wbr>token</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Lifetime in minutes of the recovery email token.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>skip_<wbr>unlock</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}When an Active Directory user is locked out of Okta, the Okta unlock operation should also attempt to unlock the user's Windows account.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>sms_<wbr>recovery</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Enable or disable SMS password recovery: ACTIVE or INACTIVE.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}











<h3>Package Details</h3>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-okta">https://github.com/pulumi/pulumi-okta</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
    
</dl>
