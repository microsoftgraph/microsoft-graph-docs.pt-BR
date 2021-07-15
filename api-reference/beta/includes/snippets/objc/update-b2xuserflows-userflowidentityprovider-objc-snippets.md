---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12741f64f9ab27c07d25819311b43bd5f14e4310
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439523"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2xUserFlows/B2X_1_Test/userflowIdentityProviders/$ref"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityProviderBase *userFlowIdentityProviders = [[MSGraphIdentityProviderBase alloc] init];

NSError *error;
NSData *userFlowIdentityProvidersData = [userFlowIdentityProviders getSerializedDataWithError:&error];
[urlRequest setHTTPBody:userFlowIdentityProvidersData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```