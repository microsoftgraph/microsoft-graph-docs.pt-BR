---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53fabab88b795aabb77846ffcbbeb6eb27170690
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322880"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSecureScoreControlProfile()
controlStateUpdates := "controlStateUpdates-value"
requestBody.SetControlStateUpdates(&controlStateUpdates)
secureScoreControlProfileId := "secureScoreControlProfile-id"
graphClient.Security().SecureScoreControlProfilesById(&secureScoreControlProfileId).Patch(requestBody)


```