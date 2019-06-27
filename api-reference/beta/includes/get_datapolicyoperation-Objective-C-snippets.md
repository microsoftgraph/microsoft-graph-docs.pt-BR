---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd4b95d33e228f9723976a174eb9d94fca92e4c1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35318063"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/dataPolicyOperations/{id}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphDataPolicyOperation *dataPolicyOperation = [[MSGraphDataPolicyOperation alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```