# IRC <--> Zulip bridge

## Usage

```
./irc-mirror.py --irc-server=IRC_SERVER --channel=<CHANNEL> --nick-prefix=<NICK> --stream=<STREAM> [optional args]
```

`--stream` is a Zulip stream.

Specify your Zulip API credentials and server in a ~/.zuliprc file or using the options.

Note that "_zulip" will be automatically appended to the IRC nick provided

## Example

```
./irc-mirror.py --irc-server=irc.freenode.net --channel='#python-mypy' --nick-prefix=irc_mirror --stream='test here' \
                --site="https://chat.zulip.org" --user=<bot-email> --api-key=<bot-api-key>
```