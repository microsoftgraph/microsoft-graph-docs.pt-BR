---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6af95c96922c089f9a5795008d2007646f30fd61
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204876"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleEligibilityScheduleInstances/8MYkhImhnkm70CbBdTyW1BbHHAdHgZdDpbqyEFlRzAs-1-e"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUnifiedRoleEligibilityScheduleInstance *unifiedRoleEligibilityScheduleInstance = [[MSGraphUnifiedRoleEligibilityScheduleInstance alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```