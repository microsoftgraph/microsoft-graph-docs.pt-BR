---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f791ba4e051464bdbc746e84ccec579751b6d470
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442078"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/tenantTags"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphManagedTenantsTenantTag *tenantTag = [[MSGraphManagedTenantsTenantTag alloc] init];
[tenantTag setDisplayName:@"Support"];
[tenantTag setDescription:@"Tenants that have purchased extended support"];

NSError *error;
NSData *tenantTagData = [tenantTag getSerializedDataWithError:&error];
[urlRequest setHTTPBody:tenantTagData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```