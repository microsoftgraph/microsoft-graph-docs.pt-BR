---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5c60758a84b1d9c329181a295c88ea48fdefaee9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086527"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCalendarPermission()
emailAddress := msgraphsdk.NewEmailAddress()
requestBody.SetEmailAddress(emailAddress)
name := "Samantha Booth"
emailAddress.SetName(&name)
address := "samanthab@adatum.onmicrosoft.com"
emailAddress.SetAddress(&address)
isInsideOrganization := true
requestBody.SetIsInsideOrganization(&isInsideOrganization)
isRemovable := true
requestBody.SetIsRemovable(&isRemovable)
role := "read"
requestBody.SetRole(&role)
options := &msgraphsdk.CalendarPermissionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Calendar().CalendarPermissions().Post(options)


```