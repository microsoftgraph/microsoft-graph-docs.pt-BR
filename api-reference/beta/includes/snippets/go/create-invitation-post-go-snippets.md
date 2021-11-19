---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9aaba3f8d9194c0b6099e1b8ed49d0458a2ac51
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094296"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewInvitation()
invitedUserEmailAddress := "admin@fabrikam.com"
requestBody.SetInvitedUserEmailAddress(&invitedUserEmailAddress)
inviteRedirectUrl := "https://myapp.contoso.com"
requestBody.SetInviteRedirectUrl(&inviteRedirectUrl)
options := &msgraphsdk.InvitationsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Invitations().Post(options)


```