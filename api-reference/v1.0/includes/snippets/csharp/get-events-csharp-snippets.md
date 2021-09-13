---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6897dbaea4f6f848262cc857a22f60c6cf8678bfc1fb136c2eeda3a014399e86
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102950"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Me.Events
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .Select("subject,body,bodyPreview,organizer,attendees,start,end,location")
    .GetAsync();

```