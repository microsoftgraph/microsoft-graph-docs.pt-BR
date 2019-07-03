---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e24362d7914a6cc5a7de9bcc9ed55cb4a6fce5d8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518242"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/tables"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *workbookTableList = [[NSMutableArray alloc] init];
        workbookTableList = [jsonFinal valueForKey:@"value"];
        MSGraphWorkbookTable *workbookTable = [[MSGraphWorkbookTable alloc] initWithDictionary:[workbookTableList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```