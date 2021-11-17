---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2844af91893edbfd7c25c387cd82596be48262f96787ef8c93b0b78b1f09d131
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213637"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{application-id}"].ExtensionProperties["{extensionProperty-id}"]
    .Request()
    .DeleteAsync();

```