---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8515e2ae1bd170a18e5375c6bba60d97a7754e9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721691"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = await graphClient.Me.MailFolders["AAMkAGVmMDEzM"]
    .Request()
    .GetAsync();

```