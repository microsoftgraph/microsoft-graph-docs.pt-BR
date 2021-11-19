---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 159ea178efc9d0fbb41177d6bd578addf4f7dfff
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087350"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
currentPassword := "xWwvJ]6NMw+bWH-d"
requestBody.SetCurrentPassword(&currentPassword)
newPassword := "0eM85N54wFxWwvJ]"
requestBody.SetNewPassword(&newPassword)
options := &msgraphsdk.ChangePasswordRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.Me().ChangePassword().Post(options)


```