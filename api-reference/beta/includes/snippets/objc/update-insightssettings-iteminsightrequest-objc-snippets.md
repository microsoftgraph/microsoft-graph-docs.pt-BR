---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9402b41fd7732d297b5d365607a8eaf60fbaceb
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339494"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization/{organizationId}/settings/itemInsights"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphInsightsSettings *insightsSettings = [[MSGraphInsightsSettings alloc] init];
[insightsSettings setDisabledForGroup:@"edbfe4fb-ec70-4300-928f-dbb2ae86c981"];

NSError *error;
NSData *insightsSettingsData = [insightsSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:insightsSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```