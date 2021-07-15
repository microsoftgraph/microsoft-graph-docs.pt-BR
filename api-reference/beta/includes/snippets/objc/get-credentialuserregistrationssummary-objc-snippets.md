---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4e41dcd22541588caef5d14309915921fc5a47e8
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440019"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/credentialUserRegistrationsSummaries/{credentialUserRegistrationsSummaryId}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphCredentialUserRegistrationsSummary *credentialUserRegistrationsSummary = [[MSGraphCredentialUserRegistrationsSummary alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```