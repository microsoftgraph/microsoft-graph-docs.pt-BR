---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef2788c6ea0b4645f6f17ac7b9231b2813111dfba0b8d5289e2562794e974a93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898103"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.administrativeUnits("{id}").scopedRoleMembers("{id}")
    .buildRequest()
    .delete();

```