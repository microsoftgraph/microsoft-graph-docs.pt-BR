---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79617b6ad1a8d165e284439cece673bf88406b92
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084501"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).InstalledApps().Get(options)


```