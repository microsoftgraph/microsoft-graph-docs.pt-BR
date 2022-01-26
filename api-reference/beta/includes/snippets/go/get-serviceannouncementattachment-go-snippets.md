---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 927e9e1459947184844305a7bf280686d931fb9d
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225776"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

serviceUpdateMessageId := "serviceUpdateMessage-id"
serviceAnnouncementAttachmentId := "serviceAnnouncementAttachment-id"
graphClient.Admin().ServiceAnnouncement().MessagesById(&serviceUpdateMessageId).AttachmentsById(&serviceAnnouncementAttachmentId).Content().Get(nil)


```