---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: edc3e36fcd566c4a6f7b8a2150a207b39d6f8bdc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324308"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userAccountInformationId := "userAccountInformation-id"
result, err := graphClient.Me().Profile().AccountById(&userAccountInformationId).Get()


```