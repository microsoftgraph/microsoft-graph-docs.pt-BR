---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7707ea152e44e310f8b96924e5193895303594be
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286761"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.TenantRelationships().ManagedTenants().CredentialUserRegistrationsSummaries().Get(nil)


```