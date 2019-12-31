---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08985efe8694ce4246e090a1ac844e0189432718
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912858"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Communications.Calls["2e1a0b00-2db4-4022-9570-243709c565ab"]
    .KeepAlive()
    .Request()
    .PostAsync();

```