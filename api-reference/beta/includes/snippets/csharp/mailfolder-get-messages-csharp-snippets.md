---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac1ba61422ed56e722e7d5411eb99556f9dc359d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879991"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.MailFolders["AAMkAGVmMDEzM"].Messages
    .Request()
    .GetAsync();

```