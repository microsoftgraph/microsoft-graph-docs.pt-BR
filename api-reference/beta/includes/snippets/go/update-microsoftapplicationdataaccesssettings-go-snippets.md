---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53cf314fb3cc60cb4eff378874039a7b9b063295
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323693"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMicrosoftApplicationDataAccessSettings()
disabledForGroup := "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
requestBody.SetDisabledForGroup(&disabledForGroup)
organizationId := "organization-id"
graphClient.OrganizationById(&organizationId).Settings().MicrosoftApplicationDataAccess().Patch(requestBody)


```