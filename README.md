# Email::Valid
Email::Valid - Check validity of email addresses
## Synopsis
```perl6
use v6;
use Email::Valid;

my $email = Email::Valid.new(:simple = True);

if $email.validate("test@domain.tld") {
    say "test@domain.tld is valid";
}
```

## Description
This module validates if given email is valid.
It's a validation only for "most" popular email types.
It allows IDN domains ( 'xn--' )

## TODO
- [ ] Add MX Check
- [ ] Add "Hello" Callback verification
- [ ] Allow quoted mailboxes
- [ ] Allow ip addresses in domain part
- [ ] Fix ( Add ) IDN domain char limit
