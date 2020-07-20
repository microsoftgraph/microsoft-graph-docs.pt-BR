---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c9dc62d98f70bb745eb9028a61addb2e3cc36cde
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080671"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization/settings"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphOrganization *organization = [[MSGraphOrganization alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```