---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7d7f1d5b99d854afe4fe67ab4254b7677889bc2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324514"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tenantTagId := "tenantTag-id"
graphClient.TenantRelationships().ManagedTenants().TenantTagsById(&tenantTagId).Delete()


```