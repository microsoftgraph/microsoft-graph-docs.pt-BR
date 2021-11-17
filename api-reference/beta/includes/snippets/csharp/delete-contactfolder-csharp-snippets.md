---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55458f775ef9b49ee41e3a30c1e0144a43c38431f6848a9e987b58f348117d58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.ContactFolders["{contactFolder-id}"]
    .Request()
    .DeleteAsync();

```