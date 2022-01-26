---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 130e37adf56f1884e8a69b55666cae6799e05137
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225959"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

serviceUpdateMessageId := "serviceUpdateMessage-id"
graphClient.Admin().ServiceAnnouncement().MessagesById(&serviceUpdateMessageId).AttachmentsArchive().Get(nil)


```