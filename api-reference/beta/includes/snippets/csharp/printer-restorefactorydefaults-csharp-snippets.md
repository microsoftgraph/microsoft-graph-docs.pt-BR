---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd6a03569c69ab28344ed9c4f757c8459290d1d6
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782725"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{id}"]
    .RestoreFactoryDefaults()
    .Request()
    .PostAsync();

```