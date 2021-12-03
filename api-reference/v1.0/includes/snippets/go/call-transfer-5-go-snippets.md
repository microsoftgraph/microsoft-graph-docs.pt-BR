---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9efc4569cad3ba8b4ff8fd6606566bf3995e0d3c
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287272"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
graphClient.Communications().CallsById(&callId).Transfer().Post(nil)


```