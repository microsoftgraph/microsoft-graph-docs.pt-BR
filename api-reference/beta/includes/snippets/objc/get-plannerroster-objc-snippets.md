---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a64925ca9a01236b6c10771f960a8635507aec8bbb50af944ee2bb4767c0ffc4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271925"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/rosters/6519868f-868f-6519-8f86-19658f861965"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphPlannerRoster *plannerRoster = [[MSGraphPlannerRoster alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```