---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72d7afad476b99d585abb56b74eb89aaed31746f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323977"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTag()
description := "This is an updated description."
requestBody.SetDescription(&description)
caseId := "case-id"
tagId := "tag-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).TagsById(&tagId).Patch(requestBody)


```