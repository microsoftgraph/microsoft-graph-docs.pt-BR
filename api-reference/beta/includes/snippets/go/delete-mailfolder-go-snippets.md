---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70115bd64568d9fabb45711f0aa7115fb397e84a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094041"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

mailFolderId := "mailFolder-id"
graphClient.Me().MailFoldersById(&mailFolderId).Delete(options)


```