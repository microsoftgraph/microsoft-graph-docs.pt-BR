---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a43dedd654f67a7c8ffa84931476526a2f44bb44
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538417"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUser *user = [[MSGraphUser alloc] init];
[user setDisplayName:@"John Smith"];
NSMutableArray *identitiesList = [[NSMutableArray alloc] init];
MSGraphObjectIdentity *identities = [[MSGraphObjectIdentity alloc] init];
[identities setSignInType:@"userName"];
[identities setIssuer:@"contoso.onmicrosoft.com"];
[identities setIssuerAssignedId:@"johnsmith"];
[identitiesList addObject: identities];
MSGraphObjectIdentity *identities = [[MSGraphObjectIdentity alloc] init];
[identities setSignInType:@"federated"];
[identities setIssuer:@"facebook.com"];
[identities setIssuerAssignedId:@"5eecb0cd"];
[identitiesList addObject: identities];
[user setIdentities:identitiesList];
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