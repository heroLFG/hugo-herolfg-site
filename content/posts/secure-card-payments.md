+++ 
draft = false
date = 2020-10-04T05:23:08-05:00
title = "Secure Card Payments"
description = "How a debit or credit card could work better in the future."
slug = "secure-card-payments" 
tags = ['finance','innovation','security','payments']
categories = ['innovation','finance']
externalLink = ""
series = []
+++

My wife checked our bank account this morning and discovered that our debit card had been used by a thief.  I verified that the card was in my wallet.  I called my bank and cancelled the card so that the thief would not be able to use it again.  And I created a dispute for the charge on my bank's website.

My first thought was that the merchant should be responsible for this kind of thing.  How did they allow someone to use a card that didn't belong to them?  I eventually calmed down and thought about how I might avoid this problem in the future.  And the answer is related to [privacy.com](https://privacy.com/pricing) and multi factor authentication.

My business idea is to allow people to create and control their own payment cards.  My idea is based on the idea being offered by privacy.com which allows you to create virtual cards.  The big difference is that I should be able to have a real card sent to me in the mail which is the physical representation of the virtual card.

My goal is to receive an SMS text message any time someone tries to use my card.  I can then respond to that text message in order to accept or decline the attempted transaction.

I think privacy.com could offer this service or a 3rd party like myself could integrate with privacy.com and offer this service.

My initial thoughts on implementation details is that the virtual card could have a spend limit which will always decline until the text message response is received by the owner of the card.  The spend limit would be increased on the virtual card and then the payment could occur.  Another option is to allow a white list of merchants such that the merchant is not allowed until the text message response is received.  This may require that the merchant retry the card after the text message response has been received.