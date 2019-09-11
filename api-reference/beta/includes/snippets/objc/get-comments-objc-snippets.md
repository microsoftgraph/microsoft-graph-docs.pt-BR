---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db60686eb44ca4f9a196a0cae118c21c45430440
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838855"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/drive/root/workbook/comments"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *workbookCommentList = [[NSMutableArray alloc] init];
        workbookCommentList = [jsonFinal valueForKey:@"value"];
        MSGraphWorkbookComment *workbookComment = [[MSGraphWorkbookComment alloc] initWithDictionary:[workbookCommentList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```