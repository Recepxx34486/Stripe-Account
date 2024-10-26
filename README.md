# Stripe-Account
// Set your secret key. Remember to switch to your live secret key in production.
// See your keys here: https://dashboard.stripe.com/apikeys
StripeConfiguration.ApiKey = "sk_test_51QDGlEAsFzkudd3Qf17EXUcFI5ghXdFN7XFtpE2Gb2zOzA89hldydow06nyfz9YCLfey4GDNASRmghrEurRNdlJD00Fhtd3Htr";

var options = new Stripe.Terminal.LocationCreateOptions
{
    DisplayName = "HQ",
    Address = new AddressOptions
    {
        Line1 = "1272 Valencia Street",
        City = "San Francisco",
        State = "CA",
        Country = "US",
        PostalCode = "94110",
    },
};
var requestOptions = new RequestOptions
{
    StripeAccount = "{{CONNECTED_ACCOUNT_ID}}",
};
var service = new Stripe.Terminal.LocationService();
service.Create(options, requestOptions);

"sk_test_51QDGlEAsFzkudd3Qf17EXUcFI5ghXdFN7XFtpE2Gb2zOzA89hldydow06nyfz9YCLfey4GDNASRmghrEurRNdlJD00Fhtd3Htr:" \
  -H "Stripe-Account: {{CONNECTED_ACCOUNT_ID}}" \
  -d display_name=HQ \
  -d "address[line1]"="1272 Valencia Street" \
  -d "address[city]"="San Francisco" \
  -d "address[state]"=CA \
  -d "address[country]"=US \
  -d "address[postal_code]"=94110
// Set your secret key. Remember to switch to your live secret key in production.
// See your keys here: https://dashboard.stripe.com/apikeys
StripeConfiguration.ApiKey = "sk_test_51QDGlEAsFzkudd3Qf17EXUcFI5ghXdFN7XFtpE2Gb2zOzA89hldydow06nyfz9YCLfey4GDNASRmghrEurRNdlJD00Fhtd3Htr";

var options = new Stripe.Terminal.ReaderCreateOptions
{
    RegistrationCode = "{{READER_REGISTRATION_CODE}}",
    Label = "Alice's reader",
    Location = "{{LOCATION_ID}}",
};
var requestOptions = new RequestOptions
{
    StripeAccount = "{{CONNECTED_ACCOUNT_ID}}",
};
var service = new Stripe.Terminal.ReaderService();
service.Create(options, requestOptions);
// Set your secret key. Remember to switch to your live secret key in production.
// See your keys here: https://dashboard.stripe.com/apikeys
StripeConfiguration.ApiKey = "sk_test_51QDGlEAsFzkudd3Qf17EXUcFI5ghXdFN7XFtpE2Gb2zOzA89hldydow06nyfz9YCLfey4GDNASRmghrEurRNdlJD00Fhtd3Htr";

var options = new Stripe.Terminal.ConnectionTokenCreateOptions
{
    Location = "{{LOCATION_ID}}",
};
var requestOptions = new RequestOptions
{
    StripeAccount = "{{CONNECTED_ACCOUNT_ID}}",
};
var service = new Stripe.Terminal.ConnectionTokenService();
service.Create(options, requestOptions);
// Set your secret key. Remember to switch to your live secret key in production.
// See your keys here: https://dashboard.stripe.com/apikeys
StripeConfiguration.ApiKey = "sk_test_51QDGlEAsFzkudd3Qf17EXUcFI5ghXdFN7XFtpE2Gb2zOzA89hldydow06nyfz9YCLfey4GDNASRmghrEurRNdlJD00Fhtd3Htr";

var options = new PaymentIntentCreateOptions
{
    Amount = 1000,
    Currency = "usd",
    PaymentMethodTypes = new List<string> { "card_present" },
    CaptureMethod = "manual",
};
var requestOptions = new RequestOptions
{
    StripeAccount = "{{CONNECTED_ACCOUNT_ID}}",
};
var service = new PaymentIntentService();
service.Create(options, requestOptions);
// Set your secret key. Remember to switch to your live secret key in production.
// See your keys here: https://dashboard.stripe.com/apikeys
StripeConfiguration.ApiKey = "sk_test_51QDGlEAsFzkudd3Qf17EXUcFI5ghXdFN7XFtpE2Gb2zOzA89hldydow06nyfz9YCLfey4GDNASRmghrEurRNdlJD00Fhtd3Htr";

var options = new Stripe.Terminal.LocationCreateOptions
{
    DisplayName = "HQ",
    Address = new AddressOptions
    {
        Line1 = "1272 Valencia Street",
        City = "San Francisco",
        State = "CA",
        Country = "US",
        PostalCode = "94110",
    },
};
var service = new Stripe.Terminal.LocationService();
service.Create(options);
// Set your secret key. Remember to switch to your live secret key in production.
// See your keys here: https://dashboard.stripe.com/apikeys
StripeConfiguration.ApiKey = "sk_test_51QDGlEAsFzkudd3Qf17EXUcFI5ghXdFN7XFtpE2Gb2zOzA89hldydow06nyfz9YCLfey4GDNASRmghrEurRNdlJD00Fhtd3Htr";

var options = new Stripe.Terminal.ReaderCreateOptions
{
    RegistrationCode = "{{READER_REGISTRATION_CODE}}",
    Label = "Alice's reader",
    Location = "{{LOCATION_ID}}",
};
var service = new Stripe.Terminal.ReaderService();
service.Create(options);
// Set your secret key. Remember to switch to your live secret key in production.
// See your keys here: https://dashboard.stripe.com/apikeys
StripeConfiguration.ApiKey = "sk_test_51QDGlEAsFzkudd3Qf17EXUcFI5ghXdFN7XFtpE2Gb2zOzA89hldydow06nyfz9YCLfey4GDNASRmghrEurRNdlJD00Fhtd3Htr";

var options = new PaymentIntentCreateOptions
{
    Amount = 1000,
    Currency = "usd",
    PaymentMethodTypes = new List<string> { "card_present" },
    CaptureMethod = "manual",
};
var requestOptions = new RequestOptions
{
    StripeAccount = "{{CONNECTED_ACCOUNT_ID}}",
};
var service = new PaymentIntentService();
service.Create(options, requestOptions);
// Set your secret key. Remember to switch to your live secret key in production.
// See your keys here: https://dashboard.stripe.com/apikeys
StripeConfiguration.ApiKey = "sk_test_51QDGlEAsFzkudd3Qf17EXUcFI5ghXdFN7XFtpE2Gb2zOzA89hldydow06nyfz9YCLfey4GDNASRmghrEurRNdlJD00Fhtd3Htr";

var options = new Stripe.Terminal.ReaderProcessPaymentIntentOptions
{
    PaymentIntent = "{{PAYMENT_INTENT_ID}}",
};
var service = new Stripe.Terminal.ReaderService();
service.ProcessPaymentIntent("{{READER_ID}}", options);
// Set your secret key. Remember to switch to your live secret key in production.
// See your keys here: https://dashboard.stripe.com/apikeys
StripeConfiguration.ApiKey = "sk_test_51QDGlEAsFzkudd3Qf17EXUcFI5ghXdFN7XFtpE2Gb2zOzA89hldydow06nyfz9YCLfey4GDNASRmghrEurRNdlJD00Fhtd3Htr";

var options = new Stripe.Terminal.LocationCreateOptions
{
    DisplayName = "HQ",
    Address = new AddressOptions
    {
        Line1 = "1272 Valencia Street",
        City = "San Francisco",
        State = "CA",
        Country = "US",
        PostalCode = "94110",
    },
};
var service = new Stripe.Terminal.LocationService();
service.Create(options);
  
