---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f79cfba22d4ee1c41b706b930ee61bd1f2d011105a75497aa88517986e95a20c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272509"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directory/administrativeUnits/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAdministrativeUnit *administrativeUnit = [[MSGraphAdministrativeUnit alloc] init];
[administrativeUnit setDisplayName:@"displayName-value"];
[administrativeUnit setDescription:@"description-value"];
[administrativeUnit setVisibility:@"visibility-value"];

NSError *error;
NSData *administrativeUnitData = [administrativeUnit getSerializedDataWithError:&error];
[urlRequest setHTTPBody:administrativeUnitData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```