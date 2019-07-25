---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27ccbdeaabf03c4ddba6b3d9d641c11d6cc03177
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719418"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365ActivationsUserDetail?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365ActivationsUserDetailList = [[NSMutableArray alloc] init];
        office365ActivationsUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365ActivationsUserDetail *office365ActivationsUserDetail = [[MSGraphOffice365ActivationsUserDetail alloc] initWithDictionary:[office365ActivationsUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```