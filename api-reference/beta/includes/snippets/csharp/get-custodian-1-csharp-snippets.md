---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fba3a6c270dc42f94e35bda3fe44cce51400fb8c36e5ed7c08f2295c965fd612
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899963"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var custodians = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians
    .Request()
    .GetAsync();

```