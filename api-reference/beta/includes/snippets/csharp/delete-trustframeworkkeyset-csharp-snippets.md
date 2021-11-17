---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf80897731a4e7d016c6b2b6a70661fee8f36f7f687aac7e568a985c947ef4b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159586"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TrustFramework.KeySets["{trustFrameworkKeySet-id}"]
    .Request()
    .DeleteAsync();

```