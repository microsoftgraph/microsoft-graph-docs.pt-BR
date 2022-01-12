---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce44fb0a56cbe2fe4eb4c5e537871cc851343df05516ea39525cefd7910d57aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102114"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummary"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphDeviceCompliancePolicySettingStateSummary *deviceCompliancePolicySettingStateSummary = [[MSGraphDeviceCompliancePolicySettingStateSummary alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```