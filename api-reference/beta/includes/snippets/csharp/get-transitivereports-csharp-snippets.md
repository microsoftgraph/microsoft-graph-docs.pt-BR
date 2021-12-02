---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3e12979b6804d6c74462ffd40f7488b1283e9234f7d3748dff910f5d2bcef0fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216888"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.Contacts["{orgContact-id}"].TransitiveReports.$count
    .Request()
    .GetAsync();

```