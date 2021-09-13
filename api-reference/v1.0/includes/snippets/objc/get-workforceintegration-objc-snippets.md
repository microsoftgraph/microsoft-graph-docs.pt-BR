---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19bb6cdcc0967bbfd12c9a154cb551469c27c2778214501dbaeeea3d35fdf227
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900056"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teamwork/workforceIntegrations/{workforceintegrationid}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphWorkforceIntegration *workforceIntegration = [[MSGraphWorkforceIntegration alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```