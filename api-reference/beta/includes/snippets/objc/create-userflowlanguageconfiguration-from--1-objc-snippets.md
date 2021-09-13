---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d65b8d4553d6ab20909dbd358a49632dfc5ca41718519cf3107f988b34bf9240
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157449"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUserFlowLanguageConfiguration *userFlowLanguageConfiguration = [[MSGraphUserFlowLanguageConfiguration alloc] init];
[userFlowLanguageConfiguration setId:@"es-ES"];
[userFlowLanguageConfiguration setIsEnabled: true];

NSError *error;
NSData *userFlowLanguageConfigurationData = [userFlowLanguageConfiguration getSerializedDataWithError:&error];
[urlRequest setHTTPBody:userFlowLanguageConfigurationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```