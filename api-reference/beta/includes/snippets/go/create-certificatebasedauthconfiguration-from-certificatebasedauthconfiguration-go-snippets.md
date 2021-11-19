---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19780a34eb3c5a3c9b188cb054e890399ae8e959
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097879"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "certificateAuthorities":  []Object {
    }
}
options := &msgraphsdk.CertificateBasedAuthConfigurationRequestBuilderPostOptions{
    Body: requestBody,
}
organizationId := "organization-id"
graphClient.OrganizationById(&organizationId).CertificateBasedAuthConfiguration().Post(options)


```