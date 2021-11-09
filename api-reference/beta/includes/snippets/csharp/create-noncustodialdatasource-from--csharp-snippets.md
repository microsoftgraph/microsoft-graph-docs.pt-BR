---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6bcadfedadda9ae813d04ad82a1cbfa61a50ffc
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60736628"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var noncustodialDataSourceReference = new ReferenceRequestBody
{
    ODataId = "https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246"
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"].NoncustodialSources.References
    .Request()
    .AddAsync(noncustodialDataSourceReference);

```