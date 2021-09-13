---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b10ba59133222d029f0964ea278f463584cae6cee24f4b70b5451b918222223a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899829"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphWorkbookRangeView *workbookRangeView = [[MSGraphWorkbookRangeView alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```