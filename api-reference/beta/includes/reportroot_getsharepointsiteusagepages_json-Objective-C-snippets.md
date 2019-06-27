---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f265057a7356e9085169aa350493020ca7ad387a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35328339"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSharePointSiteUsagePages(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *sharePointSiteUsagePagesList = [[NSMutableArray alloc] init];
        sharePointSiteUsagePagesList = [jsonFinal valueForKey:@"value"];
        MSGraphSharePointSiteUsagePages *sharePointSiteUsagePages = [[MSGraphSharePointSiteUsagePages alloc] initWithDictionary:[sharePointSiteUsagePagesList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```