---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49a12adef39885040650dd0a7987dda4f72a37ca
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508489"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/contactFolders"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *contactFolderList = [[NSMutableArray alloc] init];
        contactFolderList = [jsonFinal valueForKey:@"value"];
        MSGraphContactFolder *contactFolder = [[MSGraphContactFolder alloc] initWithDictionary:[contactFolderList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```