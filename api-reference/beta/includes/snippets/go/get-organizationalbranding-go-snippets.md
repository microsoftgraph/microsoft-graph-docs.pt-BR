---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7d0bc4212458c3df5ad06efbac14e67a7892d55
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090333"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Accept-Language": "0"
}
options := &msgraphsdk.BrandingRequestBuilderGetOptions{
    H: headers,
}
organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Branding().Get(options)


```