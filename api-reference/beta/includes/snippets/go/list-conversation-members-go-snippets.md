---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbf195a6cb8e106c574e0768bddb9decc9f37ff4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323916"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
result, err := graphClient.Me().ChatsById(&chatId).Members().Get()


```