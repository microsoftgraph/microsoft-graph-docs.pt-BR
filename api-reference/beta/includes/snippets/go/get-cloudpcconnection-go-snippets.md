---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58ddb76f4af1833cd16e714a8e244abed2014f7a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286742"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcConnectionId := "cloudPcConnection-id"
result, err := graphClient.TenantRelationships().ManagedTenants().CloudPcConnectionsById(&cloudPcConnectionId).Get(nil)


```