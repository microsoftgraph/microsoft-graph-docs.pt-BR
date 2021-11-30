---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f223c3366f9ad71b317cd3bba0029834bd2c5c9f
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224572"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customSecurityAttributeDefinitions = await graphClient.Directory.CustomSecurityAttributeDefinitions
    .Request()
    .Filter("attributeSet eq 'Engineering' and status eq 'Available' and type eq 'String'")
    .GetAsync();

```