---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 818644047d8ae7250a837937d5f9a4d2a13095a0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519241"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/taskGroups"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *outlookTaskGroupList = [[NSMutableArray alloc] init];
        outlookTaskGroupList = [jsonFinal valueForKey:@"value"];
        MSGraphOutlookTaskGroup *outlookTaskGroup = [[MSGraphOutlookTaskGroup alloc] initWithDictionary:[outlookTaskGroupList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```