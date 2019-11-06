---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 724610ca68bf1e90852c92752afc1076700e2918
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999141"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/applications/{id}/extensionProperties"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *extensionPropertyList = [[NSMutableArray alloc] init];
        extensionPropertyList = [jsonFinal valueForKey:@"value"];
        MSGraphExtensionProperty *extensionProperty = [[MSGraphExtensionProperty alloc] initWithDictionary:[extensionPropertyList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```