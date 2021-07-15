---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 300e28da9536ede03c62013ea851e85242fc6098
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440902"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *tenantGroupId = @"String";
payloadDictionary[@"tenantGroupId"] = tenantGroupId;

NSString *tenantId = @"String";
payloadDictionary[@"tenantId"] = tenantId;

NSString *managementActionId = @"String";
payloadDictionary[@"managementActionId"] = managementActionId;

NSString *managementTemplateId = @"String";
payloadDictionary[@"managementTemplateId"] = managementTemplateId;

NSString *status = @"String";
payloadDictionary[@"status"] = status;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```