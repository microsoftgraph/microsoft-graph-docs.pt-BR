---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da089845356c60cd5fcfed335235ce5d6731277a
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60729847"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"]]];
[urlRequest setHTTPMethod:@"GET"];
[urlRequest setValue:@"\"My Friendly Client\"" forHTTPHeaderField:@"ocp-client-name"];
[urlRequest setValue:@"\"1.2\"" forHTTPHeaderField:@"ocp-client-version"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphBitlockerRecoveryKey *bitlockerRecoveryKey = [[MSGraphBitlockerRecoveryKey alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```