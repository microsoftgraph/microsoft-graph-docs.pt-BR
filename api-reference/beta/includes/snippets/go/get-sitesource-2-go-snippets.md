---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23cf5fbeed09d56ddad99da9a5d0883372559e9a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60998575"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

caseId := "case-id"
custodianId := "custodian-id"
siteSourceId := "siteSource-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).SiteSourcesById(&siteSourceId).Get(options)


```