---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1276eef0b5fa55fc310c94ed2c8e441c55758d4f28f3fee4306cc0cfa13a32a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216043"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["{educationSchool-id}"]
    .Request()
    .DeleteAsync();

```