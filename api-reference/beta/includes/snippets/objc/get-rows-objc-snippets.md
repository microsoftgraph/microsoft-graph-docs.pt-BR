---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8d487e78e5bf4f3e455ed3c76fab5530d4fa0f7f
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997431"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/rows"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *workbookRangeViewList = [[NSMutableArray alloc] init];
        workbookRangeViewList = [jsonFinal valueForKey:@"value"];
        MSGraphWorkbookRangeView *workbookRangeView = [[MSGraphWorkbookRangeView alloc] initWithDictionary:[workbookRangeViewList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```