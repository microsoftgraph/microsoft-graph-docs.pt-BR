---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59a1cdae64d563a7bf199ade0446285777471ba0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337303"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

servicePrincipalRiskDetectionId := "servicePrincipalRiskDetection-id"
result, err := graphClient.IdentityProtection().ServicePrincipalRiskDetectionsById(&servicePrincipalRiskDetectionId).Get(nil)


```