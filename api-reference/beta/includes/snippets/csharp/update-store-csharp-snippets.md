---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 306ddacdd6c72c3a229361bb5a4e8e083fea16b3057b0e15c0f4317574857e47
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272649"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var store = new Microsoft.Graph.TermStore.Store
{
    DefaultLanguageTag = "en-US"
};

await graphClient.TermStore
    .Request()
    .UpdateAsync(store);

```