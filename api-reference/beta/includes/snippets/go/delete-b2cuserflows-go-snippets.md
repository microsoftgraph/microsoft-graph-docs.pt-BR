---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 229e393b74c05a6558b0cbc2224f899ae99f8fc1
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285975"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).Delete(nil)


```