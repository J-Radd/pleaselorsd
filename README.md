# pleaselorsd
// Set your secret key. Remember to switch to your live secret key in production!
// See your keys here: https://dashboard.stripe.com/account/apikeys
StripeConfiguration.ApiKey = "sk_live_...4kUR";

var options = new CardCreateOptions
{
  Cardholder = "acct_1HniFF2UNLGLziCb",
  Type = "virtual",
  Currency = "cad",
};

var service = new CardService();
var card = service.Create(options);
