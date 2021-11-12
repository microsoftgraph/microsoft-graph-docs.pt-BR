---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de34baadf84c11d1693c80034cd117ca60bb8078a279083c6284439498697ad8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274791"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.TaskDefinitions["{printTaskDefinition-id}"]
    .Request()
    .DeleteAsync();

```