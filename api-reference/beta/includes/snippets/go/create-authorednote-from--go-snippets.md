---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b378e56a33ffef761e1f80098a2cbf6c37d99385
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719080"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthoredNote()
content := msgraphsdk.NewItemBody()
requestBody.SetContent(content)
content := "Please take a look at the files tagged with follow up"
content.SetContent(&content)
contentType := "text"
content.SetContentType(&contentType)
subjectRightsRequestId := "subjectRightsRequest-id"
result, err := graphClient.Privacy().SubjectRightsRequestsById(&subjectRightsRequestId).Notes().Post(requestBody)


```