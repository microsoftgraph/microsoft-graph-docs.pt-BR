---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0a661a3e928efd39f1f790b943dfad29a5fe34328775aeb8f321709cb3c9f187
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216827"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{id}/teamwork/installedApps/{id}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUserScopeTeamsAppInstallation *userScopeTeamsAppInstallation = [[MSGraphUserScopeTeamsAppInstallation alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```