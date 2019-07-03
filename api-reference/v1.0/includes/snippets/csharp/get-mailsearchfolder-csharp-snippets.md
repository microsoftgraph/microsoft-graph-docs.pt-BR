---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 05ab5754a0baed2a67836625b8e0c5de10f31786
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508366"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = await graphClient.Me.MailFolders["AAMkAGVmMDEzN"]
    .Request()
    .GetAsync();

```