---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e85dbca9d4b4b2202819829ee725738f93b072d642a97902c0870df0ba429f50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213960"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolders = await graphClient.Me.MailFolders
    .Request()
    .GetAsync();

```