---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65aa9cdfc7c7ec6b6fcc90c4e15c945bc38f3dc406d91ed5625ddfc8d732fbb9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.AdministrativeUnits["{administrativeUnit-id}"]
    .Request()
    .DeleteAsync();

```