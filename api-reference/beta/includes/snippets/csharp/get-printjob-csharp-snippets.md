---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2237b830daa4638df6cabdbd0d2945fad88e59363ffe636baaa64108df6c2b1d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100432"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printJob = await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"]
    .Request()
    .GetAsync();

```