---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9db55c229a9766e01e3b904bf41f78316c59f7ab16f193f4dda5907f1f17be40
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156316"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectors = await graphClient.Print.Printers["{printer-id}"].Connectors
    .Request()
    .GetAsync();

```