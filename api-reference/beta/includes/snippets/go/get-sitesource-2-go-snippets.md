---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26b971eb2ad44d6f7f176cf626e1cbcb27a8afbc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094098"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
custodianId := "custodian-id"
siteSourceId := "siteSource-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).SiteSourcesById(&siteSourceId).Get(options)


```