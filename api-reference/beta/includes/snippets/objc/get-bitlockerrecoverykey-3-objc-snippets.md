---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 027bc6acd0b6bb707d62d3195bc165de9c9acd38
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944317"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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