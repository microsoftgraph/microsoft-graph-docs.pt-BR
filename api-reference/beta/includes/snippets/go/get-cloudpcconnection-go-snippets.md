---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eee5040e95c6e4a6cf12ed2cff17aae206297661
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322487"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcConnectionId := "cloudPcConnection-id"
result, err := graphClient.TenantRelationships().ManagedTenants().CloudPcConnectionsById(&cloudPcConnectionId).Get()


```