---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6a90807d4f244f770413be2b6a197f0247fdc5b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323365"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "certificateAuthorities":  []Object {
    }
}
organizationId := "organization-id"
graphClient.OrganizationById(&organizationId).CertificateBasedAuthConfiguration().Post(requestBody)


```