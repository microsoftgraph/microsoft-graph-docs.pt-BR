---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa7012bccbd5a730bdf369eb4b3804662603f770
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753087"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/configuration"]]];
[urlRequest setHTTPMethod:@"POST"];

MSGraphPrintJobConfiguration *printJobConfiguration = [[MSGraphPrintJobConfiguration alloc] init];
[printJobConfiguration setFeedOrientation: [MSGraphPrinterFeedOrientation longEdgeFirst]];
NSMutableArray *pageRangesList = [[NSMutableArray alloc] init];
MSGraphIntegerRange *pageRanges = [[MSGraphIntegerRange alloc] init];
[pageRanges setStart: 1];
[pageRanges setEnd: 1];
[pageRangesList addObject: pageRanges];
[printJobConfiguration setPageRanges:pageRangesList];
[printJobConfiguration setQuality: [MSGraphPrintQuality medium]];
[printJobConfiguration setDpi: 600];
[printJobConfiguration setOrientation: [MSGraphPrintOrientation landscape]];
[printJobConfiguration setCopies: 1];
[printJobConfiguration setDuplexMode: [MSGraphPrintDuplexMode oneSided]];
[printJobConfiguration setColorMode: [MSGraphPrintColorMode blackAndWhite]];
[printJobConfiguration setInputBin:@"by-pass-tray"];
[printJobConfiguration setOutputBin:@"output-tray"];
[printJobConfiguration setMediaSize:@"A4"];
MSGraphPrintMargin *margin = [[MSGraphPrintMargin alloc] init];
[margin setTop: 0];
[margin setBottom: 0];
[margin setLeft: 0];
[margin setRight: 0];
[printJobConfiguration setMargin:margin];
[printJobConfiguration setMediaType:@"stationery"];
[printJobConfiguration setFinishings: null];
[printJobConfiguration setPagesPerSheet: 1];
[printJobConfiguration setMultipageLayout: [MSGraphPrintMultipageLayout clockwiseFromBottomLeft]];
[printJobConfiguration setCollate: false];
[printJobConfiguration setScaling: [MSGraphPrintScaling shrinkToFit]];
[printJobConfiguration setFitPdfToPage: false];

NSError *error;
NSData *printJobConfigurationData = [printJobConfiguration getSerializedDataWithError:&error];
[urlRequest setHTTPBody:printJobConfigurationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```