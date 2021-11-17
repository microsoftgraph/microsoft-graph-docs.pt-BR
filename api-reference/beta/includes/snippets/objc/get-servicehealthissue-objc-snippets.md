---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5668113412b7e46c58da3892f65ef1e0e2ad9150c95ee062f32970a7c055f5ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272657"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/admin/serviceAnnouncement/issues/MO226784"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphServiceHealthIssue *serviceHealthIssue = [[MSGraphServiceHealthIssue alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```