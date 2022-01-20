---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 883b953b15c75bdf19e4ead01964b11401d28b58
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137587"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Planner().All().Delta()().Get(nil)


```