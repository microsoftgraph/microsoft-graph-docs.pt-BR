---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0a56830b9406a2e5422115599f5745ea158cb828
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324518"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

credentialUserRegistrationsSummaryId := "credentialUserRegistrationsSummary-id"
result, err := graphClient.TenantRelationships().ManagedTenants().CredentialUserRegistrationsSummariesById(&credentialUserRegistrationsSummaryId).Get()


```