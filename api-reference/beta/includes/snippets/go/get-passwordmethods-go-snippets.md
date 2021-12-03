---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fba83d4606bcbf380a7d5ed0521cd4e472c0b951
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285981"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Authentication().PasswordMethods().Get(nil)


```