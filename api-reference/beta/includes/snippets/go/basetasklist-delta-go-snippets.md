---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: faf84432158bb8f97c0c7d847ab6fc6414fe5ab7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094873"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Tasks().Lists().Delta()().Get(nil)


```