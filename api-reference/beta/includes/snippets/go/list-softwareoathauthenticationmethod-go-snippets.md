---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6695652c75a9c6c4b1c2190e01a186038f86cca
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285980"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Authentication().SoftwareOathMethods().Get(nil)


```