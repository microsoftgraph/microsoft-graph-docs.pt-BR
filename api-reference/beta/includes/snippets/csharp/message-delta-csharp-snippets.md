---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc7a4d3e1db4fb39cb2ab447f7e9e5edee4f53da
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879639"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.MailFolders["{id}"].Messages
    .Delta()
    .Request()
    .GetAsync();

```