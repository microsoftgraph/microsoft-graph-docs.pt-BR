---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 765d7ed81df70697181f4e469111f8194d9c6da5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324667"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcDeviceId := "cloudPcDevice-id"
result, err := graphClient.TenantRelationships().ManagedTenants().CloudPcDevicesById(&cloudPcDeviceId).Get()


```