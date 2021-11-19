---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 011a2a0bcb465c7ce8b189c464957f5884c7e6ee
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103741"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonName()
displayName := "Innocenty Popov"
requestBody.SetDisplayName(&displayName)
first := "Innocenty"
requestBody.SetFirst(&first)
initials := "IP"
requestBody.SetInitials(&initials)
last := "Popov"
requestBody.SetLast(&last)
languageTag := "en-US"
requestBody.SetLanguageTag(&languageTag)
requestBody.SetMaiden(nil)
options := &msgraphsdk.NamesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Names().Post(options)


```