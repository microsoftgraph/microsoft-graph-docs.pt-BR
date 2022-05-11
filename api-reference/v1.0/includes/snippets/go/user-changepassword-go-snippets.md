---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f77360ec9a4499e8ce031270732ea9df289ed7ad
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325391"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
currentPassword := "xWwvJ]6NMw+bWH-d"
requestBody.SetCurrentPassword(&currentPassword)
newPassword := "0eM85N54wFxWwvJ]"
requestBody.SetNewPassword(&newPassword)
graphClient.Me().ChangePassword().Post(requestBody)


```