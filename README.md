# MailChimp API v3.0 Example

This ia a Mailchimp API 3 example using PHP and cURL. I made this for a client, took a while because their documentation is horrible, though maybe they improved it by the time you read this.

My collegue wanted a file he could post data to, this file would then execute MailChimp API calls.

## Usage

The php file takes POSTed arguments. There are 5 functions in this file:

- Adding a subscriber 'mc_subscribe();'
- Changing a subscriber fname merge tag 'mc_changename();'
- Adding someone to an interest group 'mc_addinterest();'
- Removing a subscriber from an interest group 'mc_reminterest();'
- Checking if a subscriber exists (returns 'subscribed' or '404')

Check the file to see what arguments are needed for these separate functions.

### Post tester

The post tester file can be used to test queries from your broswer. It's a form to post to the actor php.

## Variables you need to set

At the top of the file you need to set:

- Your API key from MailChimp
- Your MailChimp server prefix (e.g. us1.)

## Debug and testing

If you set the posted $_POST["debug"] to true the MailChimp API response if outputted into the screen.

## License

Use this as you will. Tweet me as thanks at <a href="https://www.twitter.com/actuallymentor">@ActuallyMentor</a>.
