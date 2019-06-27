---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3d66a6dc7681ed0c303ff3f523b0503534d9927
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35329025"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{site-id}/pages"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *sitePageList = [[NSMutableArray alloc] init];
        sitePageList = [jsonFinal valueForKey:@"value"];
        MSGraphSitePage *sitePage = [[MSGraphSitePage alloc] initWithDictionary:[sitePageList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```