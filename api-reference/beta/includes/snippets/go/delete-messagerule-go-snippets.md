---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a53536b1540a262ff81b188ae53558248c1e654c
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286439"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

mailFolderId := "mailFolder-id"
messageRuleId := "messageRule-id"
graphClient.Me().MailFoldersById(&mailFolderId).MessageRulesById(&messageRuleId).Delete(nil)


```