---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 46146595a490febd841c5dcb385c79fbf7678a5795c58d39782b8e2c1e548174
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159339"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/tables/{id|name}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookTable *workbookTable = [[MSGraphWorkbookTable alloc] init];
[workbookTable setName:@"name-value"];
[workbookTable setShowHeaders: true];
[workbookTable setShowTotals: true];
[workbookTable setStyle:@"style-value"];

NSError *error;
NSData *workbookTableData = [workbookTable getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookTableData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```