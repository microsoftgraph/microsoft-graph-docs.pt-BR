---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3859fc63c4f7987cbe7984b683a330074777a98d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466390"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookChartLegend *workbookChartLegend = [[MSGraphWorkbookChartLegend alloc] init];
[workbookChartLegend setVisible: true];
[workbookChartLegend setPosition:@"position-value"];
[workbookChartLegend setOverlay: true];

NSError *error;
NSData *workbookChartLegendData = [workbookChartLegend getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookChartLegendData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```