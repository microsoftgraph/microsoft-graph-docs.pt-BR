---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8208e25d35a5478f5e00e707820ab3694891ab96
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322726"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDisplayNameRequestBody()
displayName := "testProperties"
requestBody.SetDisplayName(&displayName)
applicationTemplateId := "applicationTemplate-id"
result, err := graphClient.ApplicationTemplatesById(&applicationTemplateId).Instantiate(applicationTemplate-id).Post(requestBody)


```