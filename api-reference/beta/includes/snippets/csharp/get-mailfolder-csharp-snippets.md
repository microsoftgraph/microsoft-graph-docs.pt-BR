---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8515e2ae1bd170a18e5375c6bba60d97a7754e9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517474"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = await graphClient.Me.MailFolders["AAMkAGVmMDEzM"]
    .Request()
    .GetAsync();

```