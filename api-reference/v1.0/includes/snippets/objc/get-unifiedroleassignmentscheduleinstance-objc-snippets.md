---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 728106d9d26103634e1a33671650e87e2fabf7cc
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205237"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleAssignmentScheduleInstances/lAPpYvVpN0KRkAEhdxReEJ2SvT9WjGJEhR4OuaezoqU-1"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUnifiedRoleAssignmentScheduleInstance *unifiedRoleAssignmentScheduleInstance = [[MSGraphUnifiedRoleAssignmentScheduleInstance alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```