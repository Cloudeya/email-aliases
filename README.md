# Set e-mail aliases for OCTOPODAMI

Want to be notified for CRON, Logwatch and other system notifications? You can set up e-mail aliases using this script!

## What's OCTOPODAMI

[OCTOPODAMI](https://www.cloudeya.co.uk/oow/) WordPress Stack simplifies the development, deployment, and management of WordPress websites and applications in the cloud.

## Usage Instructions

### SSH into your instance

```bash
ssh ec2-user@<ip-address>
```

### Run the command below in your EC2 instance

```bash
curl -L https://gitlab.com/cloudeya/email-aliases/raw/master/email-aliases.sh | sudo bash -s <you@example.com>
```

* Don't forget to substitute **you@example.com** with a valid e-mail addresss. Additionally, you can remove aliases from ```/etc/aliases``` if you want to stop receiving notifications, then run ```sudo newaliases``` to create a new one.

### Common errors

```bash
/etc/aliases: line 99: root... Warning: duplicate alias name root
/etc/aliases: line 100: ec2-user... Warning: duplicate alias name ec2-user
```

## Support

Email support is available to Amazon Web Services Marketplace Customers at [cloud@vmnative.com](mailto:cloud@vmnative.com). We do not offer refunds, but you may terminate your Octopodami Optimized WordPress (OOW) Stack at any time.

## License

The script is published under [BSD 3-Clause License](license.txt).

## Copyright

(c) 2018 [Cloudeya Limited](https://www.cloudeya.co.uk).