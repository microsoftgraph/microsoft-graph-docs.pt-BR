---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e930d20db515bd92af508790658e1f94952f9b57
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659757"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUserScopeTeamsAppInstallation *userScopeTeamsAppInstallation = [[MSGraphUserScopeTeamsAppInstallation alloc] init];

NSError *error;
NSData *userScopeTeamsAppInstallationData = [userScopeTeamsAppInstallation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:userScopeTeamsAppInstallationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```