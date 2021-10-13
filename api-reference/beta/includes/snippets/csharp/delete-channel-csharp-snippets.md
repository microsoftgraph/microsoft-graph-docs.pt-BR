---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36f57e7798f6673cec4e9d74cbd5f41ba2724bfd24f021fab9adba7eb8c80cb3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160104"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Channels["{channel-id}"]
    .Request()
    .DeleteAsync();

```