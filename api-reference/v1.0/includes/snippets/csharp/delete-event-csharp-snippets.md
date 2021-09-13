---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34c690a49e95644eccb4d56f68651337b7b9e8c5135eaebb369d1db2e36962ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102452"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Events["{event-id}"]
    .Request()
    .DeleteAsync();

```