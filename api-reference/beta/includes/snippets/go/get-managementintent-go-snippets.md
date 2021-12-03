---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 817d0a5de83a44911eb06ffd59350d99c9b2a6eb
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286901"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

managementIntentId := "managementIntent-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagementIntentsById(&managementIntentId).Get(nil)


```