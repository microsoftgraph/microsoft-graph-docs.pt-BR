---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6a3fe904713d205fdcddfd89b79ba59562d5442
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286903"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

credentialUserRegistrationsSummaryId := "credentialUserRegistrationsSummary-id"
result, err := graphClient.TenantRelationships().ManagedTenants().CredentialUserRegistrationsSummariesById(&credentialUserRegistrationsSummaryId).Get(nil)


```