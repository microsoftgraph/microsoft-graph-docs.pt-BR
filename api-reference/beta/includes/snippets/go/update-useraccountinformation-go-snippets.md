---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9f0d91836ba367c87260fc076c178f7f8016753
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324038"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserAccountInformation()
countryCode := "NO"
requestBody.SetCountryCode(&countryCode)
userAccountInformationId := "userAccountInformation-id"
graphClient.Me().Profile().AccountById(&userAccountInformationId).Patch(requestBody)


```