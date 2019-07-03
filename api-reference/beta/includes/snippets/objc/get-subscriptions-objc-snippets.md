---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5c5cd973a912357fad9821074d6fa21200ff011
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498895"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/subscriptions"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *subscriptionList = [[NSMutableArray alloc] init];
        subscriptionList = [jsonFinal valueForKey:@"value"];
        MSGraphSubscription *subscription = [[MSGraphSubscription alloc] initWithDictionary:[subscriptionList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```