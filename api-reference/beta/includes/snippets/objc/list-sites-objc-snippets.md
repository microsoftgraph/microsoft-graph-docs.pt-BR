---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8ca5c8316bd4cd00457d9138faeb205928a2e1d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725159"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *siteList = [[NSMutableArray alloc] init];
        siteList = [jsonFinal valueForKey:@"value"];
        MSGraphSite *site = [[MSGraphSite alloc] initWithDictionary:[siteList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```