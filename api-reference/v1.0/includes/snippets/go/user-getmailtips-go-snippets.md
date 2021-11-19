---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1b6fcaaea25660c04c41aa1957707b5c86a3b72
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089375"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetEmailAddresses( []String {
    "danas@contoso.onmicrosoft.com",
    "fannyd@contoso.onmicrosoft.com",
}
mailTipsOptions := "automaticReplies, mailboxFullStatus"
requestBody.SetMailTipsOptions(&mailTipsOptions)
options := &msgraphsdk.GetMailTipsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().GetMailTips().Post(options)


```