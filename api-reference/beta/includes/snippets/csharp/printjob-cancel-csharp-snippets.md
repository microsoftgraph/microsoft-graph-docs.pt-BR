---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cdc84fbae554eb5589d0a686b2ae433356196c0be44877036b34f900b5bc6807
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327651"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"]
    .Cancel()
    .Request()
    .PostAsync();

```