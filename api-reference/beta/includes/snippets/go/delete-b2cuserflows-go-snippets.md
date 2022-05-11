---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6152b1c87c24e52cb2aa880254c960cbd4046fb7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322910"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).Delete()


```