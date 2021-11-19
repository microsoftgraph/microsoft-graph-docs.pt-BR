---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c9edf063fc53a06fc9fe6b1c4c12809141dd3d82
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097633"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSectionGroup()
displayName := "Section group name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.SectionGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
sectionGroupId := "sectionGroup-id"
result, err := graphClient.Me().Onenote().SectionGroupsById(&sectionGroupId).SectionGroups().Post(options)


```