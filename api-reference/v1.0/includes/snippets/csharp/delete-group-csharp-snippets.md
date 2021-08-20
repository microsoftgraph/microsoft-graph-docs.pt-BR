---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72e12879c0a664a2f7522917fbe9160cdd34bb11cead14fed3179c1750500206
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274520"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"]
    .Request()
    .DeleteAsync();

```