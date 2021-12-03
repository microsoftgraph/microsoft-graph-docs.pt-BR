---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41e8c4511ae0a51d1e50dd860cf1b8cf17e83615
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285845"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Contacts().Get(nil)


```