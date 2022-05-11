---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92a47f49f2e58ab51c1cdba4e85a3f8fa25e9db7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322481"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Contacts().Delta()().Get()


```