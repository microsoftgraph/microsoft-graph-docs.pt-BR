---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e7db63cc1403a8affe39a23bf6342b2b440af0d1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323796"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
tagId := "tag-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).TagsById(&tagId).Get()


```