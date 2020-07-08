---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 644bca5d213764b2e63c264790f155546cee1890
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080679"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profileCardProperties = await graphClient.Organization["settings"].ProfileCardProperties
    .Request()
    .GetAsync();

```