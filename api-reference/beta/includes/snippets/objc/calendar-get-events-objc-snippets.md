---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6cbb757a6928d7ea46a807576132bfd20902e7d0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865060"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/calendar/events"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *eventList = [[NSMutableArray alloc] init];
        eventList = [jsonFinal valueForKey:@"value"];
        MSGraphEvent *event = [[MSGraphEvent alloc] initWithDictionary:[eventList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```