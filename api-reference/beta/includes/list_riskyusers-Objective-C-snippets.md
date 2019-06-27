---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60d4b02a364b37e51f84bc0447ad7fee54d73840
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35328503"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/riskyUsers"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *riskyUserList = [[NSMutableArray alloc] init];
        riskyUserList = [jsonFinal valueForKey:@"value"];
        MSGraphRiskyUser *riskyUser = [[MSGraphRiskyUser alloc] initWithDictionary:[riskyUserList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```