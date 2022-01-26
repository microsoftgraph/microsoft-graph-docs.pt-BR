---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc303d8abd6bc44396792a8eb47117471ac9f2df
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225821"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{siteId}/operations/{richLongRunningOperation-ID}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphRichLongRunningOperation *richLongRunningOperation = [[MSGraphRichLongRunningOperation alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```