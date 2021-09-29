---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1f632575cc20201bfe7f0e6c6c7c16318a8f968
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996786"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var noncustodialDataSourceReference = new ReferenceRequestBody
{
    OdataId = "https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246"
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"].NoncustodialSources.References
    .Request()
    .AddAsync(noncustodialDataSourceReference);

```