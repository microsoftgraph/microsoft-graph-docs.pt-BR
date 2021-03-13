---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee0e39e9c7b34acf321e4c913a646730a0e31d43
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792691"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directReports = await graphClient.Contacts["{orgContact-id}"].DirectReports
    .Request()
    .GetAsync();

```