---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 42898908e736963fc2fa93cb57e14d252cb5e071
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286441"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityUserFlowId := "identityUserFlow-id"
result, err := graphClient.Identity().UserFlowsById(&identityUserFlowId).Get(nil)


```