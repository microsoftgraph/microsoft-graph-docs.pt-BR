---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3f07f4945b7e430f4a0a0f3b4b0c5a27bd0e4985b36b9ffcd1c552457016940
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156754"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2cUserFlows/{id}/userAttributeAssignments/getOrder"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphAssignmentOrder *assignmentOrder = [[MSGraphAssignmentOrder alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```