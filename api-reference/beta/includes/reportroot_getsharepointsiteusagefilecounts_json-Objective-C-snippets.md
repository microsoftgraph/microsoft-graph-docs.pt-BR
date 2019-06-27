---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 783b11afecb1f4f65f7e78b785c98767a723b853
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35328343"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSharePointSiteUsageFileCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *sharePointSiteUsageFileCountsList = [[NSMutableArray alloc] init];
        sharePointSiteUsageFileCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSharePointSiteUsageFileCounts *sharePointSiteUsageFileCounts = [[MSGraphSharePointSiteUsageFileCounts alloc] initWithDictionary:[sharePointSiteUsageFileCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```