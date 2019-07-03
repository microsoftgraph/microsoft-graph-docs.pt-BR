---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 615392e147337f20b85f3ab972172c302902f9d5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477143"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUser *user = [[MSGraphUser alloc] init];
[user setAccountEnabled: true];
[user setDisplayName:@"displayName-value"];
[user setMailNickname:@"mailNickname-value"];
[user setUserPrincipalName:@"upn-value@tenant-value.onmicrosoft.com"];
MSGraphPasswordProfile *passwordProfile = [[MSGraphPasswordProfile alloc] init];
[passwordProfile setForceChangePasswordNextSignIn: true];
[passwordProfile setPassword:@"password-value"];
[user setPasswordProfile:passwordProfile];

NSError *error;
NSData *userData = [user getSerializedDataWithError:&error];
[urlRequest setHTTPBody:userData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```