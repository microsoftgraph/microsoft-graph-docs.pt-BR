---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87ea2af6e796a8226c00cec17ef6e885e7caf02b6380b8fc5c7eecdd8f312530
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156372"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"].Documents["{printDocument-id}"].Content
    .Request()
    .GetAsync();

```