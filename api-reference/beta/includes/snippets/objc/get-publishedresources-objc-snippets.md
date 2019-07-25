---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94f18fefc063dce3382fb14b053d226ba44d1cb2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875060"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/onPremisesPublishingProfiles/{publishingType}/publishedResources?$expand=agentGroups"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *publishedResourceList = [[NSMutableArray alloc] init];
        publishedResourceList = [jsonFinal valueForKey:@"value"];
        MSGraphPublishedResource *publishedResource = [[MSGraphPublishedResource alloc] initWithDictionary:[publishedResourceList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```