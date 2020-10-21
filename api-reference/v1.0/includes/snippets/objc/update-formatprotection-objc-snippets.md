---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39ac44d1374a7d124e9134090e8428dde89556e9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619387"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/names/{name}/range/format/protection"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookFormatProtection *workbookFormatProtection = [[MSGraphWorkbookFormatProtection alloc] init];
[workbookFormatProtection setLocked: true];
[workbookFormatProtection setFormulaHidden: true];

NSError *error;
NSData *workbookFormatProtectionData = [workbookFormatProtection getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookFormatProtectionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```