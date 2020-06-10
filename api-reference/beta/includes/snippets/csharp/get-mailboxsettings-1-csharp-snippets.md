---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83dc2ba65dc747d1f8be3d905bf4374e038b8cc0
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683674"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var me = await graphClient.Me
    .Request()
    .Select("MailboxSettings")
    .GetAsync();

var mailboxSettings = me.MailboxSettings;

```