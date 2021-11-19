---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce12163d8361cfb3ead2c72422f3343ff83a88c9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097072"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

credentialUserRegistrationsSummaryId := "credentialUserRegistrationsSummary-id"
result, err := graphClient.TenantRelationships().ManagedTenants().CredentialUserRegistrationsSummariesById(&credentialUserRegistrationsSummaryId).Get(options)


```