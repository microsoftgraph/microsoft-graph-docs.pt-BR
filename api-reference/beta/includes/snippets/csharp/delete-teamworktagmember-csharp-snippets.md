---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0a4c0b2090773775869e4a79f1e7ed758a8eb5ade3b78986967e0c234e897a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Tags["{teamworkTag-id}"].Members["{teamworkTagMember-id}"]
    .Request()
    .DeleteAsync();

```