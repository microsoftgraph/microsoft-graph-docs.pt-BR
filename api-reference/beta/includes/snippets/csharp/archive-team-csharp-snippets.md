---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57d3919f1d5225fbdbe96e9ac1918fc65fa5097046073010f92e57a5ea09daf2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274633"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"]
    .Archive(null)
    .Request()
    .PostAsync();

```