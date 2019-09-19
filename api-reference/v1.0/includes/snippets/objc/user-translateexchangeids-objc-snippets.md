---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acd873ddc0bbaa26ccb1f594731422f44324536d
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041899"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/translateExchangeIds"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *inputIdsList = [[NSMutableArray alloc] init];
[inputIdsList addObject: @"{rest-formatted-id-1}"];
[inputIdsList addObject: @"{rest-formatted-id-2}"];
payloadDictionary[@"inputIds"] = inputIdsList;

MSGraphExchangeIdFormat *sourceIdType = [MSGraphExchangeIdFormat restId];
payloadDictionary[@"sourceIdType"] = sourceIdType;

MSGraphExchangeIdFormat *targetIdType = [MSGraphExchangeIdFormat restImmutableEntryId];
payloadDictionary[@"targetIdType"] = targetIdType;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```