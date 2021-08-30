---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f30d9c0a60f2681f70f4c6456228b736c980dfc66fbb251b5803b3972be99157
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156770"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .Filter("membershipRuleProcessingState eq 'On'")
    .Select("id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus")
    .GetAsync();

```