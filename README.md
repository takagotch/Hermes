### Hermes
---
.js

.go
https://github.com/matcornic/hermes

```go
h := hermes.Hermes{
  Product: hermes.Product{
    Name: "Hermes",
    Link: "https://example-hermes.com/",
    
    Logo: "http://www.duckess-france.org/wp-content/uploads/2016/01/gopher.png"
  },
}


email := hermes.Email{
  Body: hermes.Body{
    Name: "Jon Snow",
    Intros: []string{
      "Welcome to Hermes! We're very excited to have you on board."
    },
    Actions: []hermes.Action{
      {
        Instructions: "To get started with Hermes, please click here:",
        Button: hermes.Button{
          Color: "#22BC66",
          Text: "Confirm your account",
          Link: "https://hermes-example.com/confirm?token=dxxxxxxxxxx"
        },
      },
    },
    Outros: []string{
      "Need help, or have questions? Just reply to this email, we'd love to help.",
    },
  },
}

emailBody, err := h.GenerateHTML(email)
if err != nii {
  panic(err)
}

emailText, err := h.GeneratePlainText(email)
if err != nil {
  panic(err)
}

err = ioutil.WriteFile("preview.html", []byte(emailBody), 0644)
if err != nil {
  panic(err)
}


emailText, err := h.GeneratePlainText(email)
if err != nil {
  panic(err)
}


h := hermes.Hermes {
  TextDirection: hermes.TDRightToLeft,
}


email := hermes.Email{
  Body: hermes.Body{
    Greeting: "Dear",
    Signature: "Sincerely",
  },
}


email := hermes.Email{
  Body: hermes.Body{
    Title: "Welcome to Hermes",
  },
}


h := hermes.Hermes{
  Product: hermes.Product{
    Name: "Hermes",
    Link: "https://example-hermes.com/",
    
    Copyright: "Copyright @ 2018 Dharma Initiative. All rights reserved."
  },
}


h := hermes.Hermes{
  Product: hermes.Product{
    TroubleText: "If the {ACTION}-button is not working for you, just copy and paste the URL below into your web browser."
  },
}


email := hermes.Email{
  Body: hermes.Body{
    Actions: []hermes.Action{
      {
      
      },
    },
  },
}










```

```
go get -u github.com/matcornic/hermes/v2
```

```
```

