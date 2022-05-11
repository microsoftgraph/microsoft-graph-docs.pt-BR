---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2b5e0535d87a470588529b16dbe6c7e9ed11a8c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325049"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Settings().ContactMergeSuggestions().Get()


```