---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35aaa88c9d2b6446a1f2c64d0fbd965b2db7135e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35475809"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/drive/root/workbook/worksheets/{id}/pivotTables"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *workbookPivotTableList = [[NSMutableArray alloc] init];
        workbookPivotTableList = [jsonFinal valueForKey:@"value"];
        MSGraphWorkbookPivotTable *workbookPivotTable = [[MSGraphWorkbookPivotTable alloc] initWithDictionary:[workbookPivotTableList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```