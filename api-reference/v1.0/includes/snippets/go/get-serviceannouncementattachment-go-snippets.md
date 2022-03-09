---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba1f35d0fbdf53a5b4f59f00e7a6684b7b0829ac
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396452"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

serviceUpdateMessageId := "serviceUpdateMessage-id"
serviceAnnouncementAttachmentId := "serviceAnnouncementAttachment-id"
result, err := graphClient.Admin().ServiceAnnouncement().MessagesById(&serviceUpdateMessageId).AttachmentsById(&serviceAnnouncementAttachmentId).Content().Get(nil)


```