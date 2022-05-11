---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81c30a98fdee4926e8ee104c60d0deca9c252258
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324463"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
id := "id-value"
requestBody.SetId(&id)
groupId := "groupId-value"
requestBody.SetGroupId(&groupId)
onenotePageId := "onenotePage-id"
result, err := graphClient.Me().Onenote().PagesById(&onenotePageId).CopyToSection(onenotePage-id).Post(requestBody)


```