---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01f0ab07de0e979aaaf2fc153614c318f5cd764d
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37636926"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/events/{id}/tentativelyAccept"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *comment = @"I may not be able to make this week. How about next week?";
payloadDictionary[@"comment"] = comment;

BOOL sendResponse = YES;
payloadDictionary[@"sendResponse"] = sendResponse;

MSGraphTimeSlot *proposedNewTime = [[MSGraphTimeSlot alloc] init];
MSGraphDateTimeTimeZone *start = [[MSGraphDateTimeTimeZone alloc] init];
[start setDateTime: "2019-12-02T18:00:00"];
[start setTimeZone:@"Pacific Standard Time"];
[proposedNewTime setStart:start];
MSGraphDateTimeTimeZone *end = [[MSGraphDateTimeTimeZone alloc] init];
[end setDateTime: "2019-12-02T19:00:00"];
[end setTimeZone:@"Pacific Standard Time"];
[proposedNewTime setEnd:end];
payloadDictionary[@"proposedNewTime"] = proposedNewTime;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```