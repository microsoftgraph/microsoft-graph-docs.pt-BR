---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3d51a974ddd17ca65a6ff00b131b90087a98df8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996740"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).CertificateBasedAuthConfiguration().Get(options)


```