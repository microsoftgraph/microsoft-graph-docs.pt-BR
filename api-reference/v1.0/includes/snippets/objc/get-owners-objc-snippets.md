---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4468543e23f826e1c7f154a2f72edda0aaed8f77
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508017"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{id}/installedApps?$expand=teamsAppDefinition"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *teamsAppInstallationList = [[NSMutableArray alloc] init];
        teamsAppInstallationList = [jsonFinal valueForKey:@"value"];
        MSGraphTeamsAppInstallation *teamsAppInstallation = [[MSGraphTeamsAppInstallation alloc] initWithDictionary:[teamsAppInstallationList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```