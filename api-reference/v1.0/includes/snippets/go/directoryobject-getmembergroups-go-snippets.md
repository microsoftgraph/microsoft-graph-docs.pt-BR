---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fce23fe33ced3ff3008ca2f24923aa4e1d964c99
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084848"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
securityEnabledOnly := true
requestBody.SetSecurityEnabledOnly(&securityEnabledOnly)
options := &msgraphsdk.GetMemberGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
directoryObjectId := "directoryObject-id"
result, err := graphClient.DirectoryObjectsById(&directoryObjectId).GetMemberGroups().Post(options)


```