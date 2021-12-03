---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8ffd84b6fa707d8f217bcc8d3f14ea417796ab83
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286008"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).Delete(nil)


```