---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41f4129b912a735651ab49bc6dab7f74a397662b
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225295"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Admin.ServiceAnnouncement.Messages["{serviceUpdateMessage-id}"].AttachmentsArchive
    .Request()
    .GetAsync();

```