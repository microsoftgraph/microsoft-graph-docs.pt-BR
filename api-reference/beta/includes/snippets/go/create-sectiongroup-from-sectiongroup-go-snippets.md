---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 880d93a545d0649b2863d855cccc73a45feadc26
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322462"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "displayName": "Section group name",
}
sectionGroupId := "sectionGroup-id"
graphClient.Me().Onenote().SectionGroupsById(&sectionGroupId).SectionGroups().Post(requestBody)


```