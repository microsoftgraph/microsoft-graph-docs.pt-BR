---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1f465649c766df5b4a4d11c0abcc24ffa2efad229b7fea4d2be8c5f429a919b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897923"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var presence = await graphClient.Communications.Presences["{presence-id}"]
    .Request()
    .GetAsync();

```