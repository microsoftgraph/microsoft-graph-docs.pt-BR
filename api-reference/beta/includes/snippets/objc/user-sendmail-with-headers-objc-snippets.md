---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4c9f0f592741af689bebaccfcc70614b207dc14e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607059"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/sendMail"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphMessage *message = [[MSGraphMessage alloc] init];
[message setSubject:@"9/9/2018: concert"];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"The group represents Nevada."];
[message setBody:body];
NSMutableArray *toRecipientsList = [[NSMutableArray alloc] init];
MSGraphRecipient *toRecipients = [[MSGraphRecipient alloc] init];
MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] init];
[emailAddress setAddress:@"AlexW@contoso.OnMicrosoft.com"];
[toRecipients setEmailAddress:emailAddress];
[toRecipientsList addObject: toRecipients];
[message setToRecipients:toRecipientsList];
NSMutableArray *internetMessageHeadersList = [[NSMutableArray alloc] init];
MSGraphInternetMessageHeader *internetMessageHeaders = [[MSGraphInternetMessageHeader alloc] init];
[internetMessageHeaders setName:@"x-custom-header-group-name"];
[internetMessageHeaders setValue:@"Nevada"];
[internetMessageHeadersList addObject: internetMessageHeaders];
MSGraphInternetMessageHeader *internetMessageHeaders = [[MSGraphInternetMessageHeader alloc] init];
[internetMessageHeaders setName:@"x-custom-header-group-id"];
[internetMessageHeaders setValue:@"NV001"];
[internetMessageHeadersList addObject: internetMessageHeaders];
[message setInternetMessageHeaders:internetMessageHeadersList];
payloadDictionary[@"message"] = message;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```