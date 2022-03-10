---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8deb2f86b6250ddecc3e48c6c2347cad3b7266a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411023"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

crossTenantAccessPolicyConfigurationPartnerTenantId := "crossTenantAccessPolicyConfigurationPartner-tenantId"
result, err := graphClient.Policies().CrossTenantAccessPolicy().PartnersById(&crossTenantAccessPolicyConfigurationPartnerTenantId).Delete(nil)


```