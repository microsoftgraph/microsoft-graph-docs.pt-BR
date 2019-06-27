---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5c5cd973a912357fad9821074d6fa21200ff011
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35317728"
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