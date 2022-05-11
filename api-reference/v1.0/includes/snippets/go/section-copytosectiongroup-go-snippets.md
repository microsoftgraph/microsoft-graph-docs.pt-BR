---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2da641893c3e02f950f2b68005fd28553aa56248
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324201"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
id := "id-value"
requestBody.SetId(&id)
groupId := "groupId-value"
requestBody.SetGroupId(&groupId)
renameAs := "renameAs-value"
requestBody.SetRenameAs(&renameAs)
onenoteSectionId := "onenoteSection-id"
result, err := graphClient.Me().Onenote().SectionsById(&onenoteSectionId).CopyToSectionGroup(onenoteSection-id).Post(requestBody)


```