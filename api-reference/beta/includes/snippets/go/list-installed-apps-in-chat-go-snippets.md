---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 341cd1ca2fb518084833bf8c23414c8840c67570
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286172"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).InstalledApps().Get(nil)


```