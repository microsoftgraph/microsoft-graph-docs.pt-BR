---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55bafe9a3ab06d5e237b9f0efb720d9dc10b6041
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473517"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var me = await graphClient.Me
    .Request()
    .Select("MailboxSettings")
    .GetAsync();

var workingHours = me.MailboxSettings.WorkingHours;

```