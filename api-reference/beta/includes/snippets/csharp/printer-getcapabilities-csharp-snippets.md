---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 345dfc169cab4fc76fa6f2763940418194290586ba0c5e4fa16f1811f41b6d68
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102480"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerCapabilities = await graphClient.Print.Printers["{printer-id}"]
    .GetCapabilities()
    .Request()
    .GetAsync();

```