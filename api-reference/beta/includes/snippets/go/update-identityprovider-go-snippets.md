---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e087a06db20dd02a6f03b5c77e2efb38c4008942
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323218"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityProvider()
clientSecret := "1111111111111"
requestBody.SetClientSecret(&clientSecret)
identityProviderId := "identityProvider-id"
graphClient.IdentityProvidersById(&identityProviderId).Patch(requestBody)


```