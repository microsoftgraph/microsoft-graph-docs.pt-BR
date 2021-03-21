---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8d0bf1941a6d0a7fd63a2b290dc491ba3f3230da
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983059"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String outputName = "2020-12-06 Contoso investigation export";

String description = "Export for the Contoso investigation";

EnumSet<ExportOptions> exportOptions = EnumSet.of(ExportOptions.ORIGINAL_FILES,ExportOptions.FILE_INFO,ExportOptions.TAGS);

ExportFileStructure exportStructure = ExportFileStructure.DIRECTORY;

graphClient.compliance().ediscovery().cases("99e865fc-e29f-479a-ba83-9e58eb017103").reviewSets("e44ac2cb-f8b4-4fd8-aa1c-1391b46ba9cc")
    .export(ReviewSetExportParameterSet
        .newBuilder()
        .withOutputName(outputName)
        .withDescription(description)
        .withAzureBlobContainer(null)
        .withAzureBlobToken(null)
        .withExportOptions(exportOptions)
        .withExportStructure(exportStructure)
        .build())
    .buildRequest()
    .post();

```