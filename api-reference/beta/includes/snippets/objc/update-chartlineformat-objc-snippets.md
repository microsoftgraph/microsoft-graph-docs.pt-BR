---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62dc7940b878211d35ca1850a90a6d4b23d06cb0f2a169a77e91071814256041
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899812"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookChartLineFormat *workbookChartLineFormat = [[MSGraphWorkbookChartLineFormat alloc] init];
[workbookChartLineFormat setColor:@"color-value"];

NSError *error;
NSData *workbookChartLineFormatData = [workbookChartLineFormat getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookChartLineFormatData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```