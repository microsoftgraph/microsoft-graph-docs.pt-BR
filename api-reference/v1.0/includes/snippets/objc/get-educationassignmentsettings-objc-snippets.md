---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34fa1989344145acc3e8dbcb60c656179d918a16
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766191"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/f4a941ff-9da6-4707-ba5b-0eae93cad0b4/assignmentsettings"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphEducationAssignmentSettings *educationAssignmentSettings = [[MSGraphEducationAssignmentSettings alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```