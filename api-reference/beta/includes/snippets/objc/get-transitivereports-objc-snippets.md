---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81d65625241fe246caf1ebd840f81f16d22c5143640356a935a029531aab476b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216886"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/contacts/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphInt32 *int32 = [[MSGraphInt32 alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```