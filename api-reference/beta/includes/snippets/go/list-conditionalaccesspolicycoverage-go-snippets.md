---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0db9bf479e5b33c8b2f1bbe2b096c35c94f14fc3
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286792"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.TenantRelationships().ManagedTenants().ConditionalAccessPolicyCoverages().Get(nil)


```