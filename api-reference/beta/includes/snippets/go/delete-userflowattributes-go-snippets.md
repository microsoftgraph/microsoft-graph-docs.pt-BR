---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77c331847aaa825804a42bb8f1b82bee85872775
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324672"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityUserFlowAttributeId := "identityUserFlowAttribute-id"
graphClient.Identity().UserFlowAttributesById(&identityUserFlowAttributeId).Delete()


```