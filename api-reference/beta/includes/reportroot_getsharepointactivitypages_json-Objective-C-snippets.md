---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76f5f9ac78981ca061ce4d12cba1fb26a42a4607
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35329369"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSharePointActivityPages(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *sharePointActivityPagesList = [[NSMutableArray alloc] init];
        sharePointActivityPagesList = [jsonFinal valueForKey:@"value"];
        MSGraphSharePointActivityPages *sharePointActivityPages = [[MSGraphSharePointActivityPages alloc] initWithDictionary:[sharePointActivityPagesList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```