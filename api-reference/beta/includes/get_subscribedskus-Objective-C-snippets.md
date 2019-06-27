---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8e5bb77156479976fc3b447558985adea10def6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35329397"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/subscribedSkus"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *subscribedSkuList = [[NSMutableArray alloc] init];
        subscribedSkuList = [jsonFinal valueForKey:@"value"];
        MSGraphSubscribedSku *subscribedSku = [[MSGraphSubscribedSku alloc] initWithDictionary:[subscribedSkuList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```