---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab168fae6649342bb8688fa3cdcd30ef19d99e61
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402771"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = false;

graphClient.groups("{id}")
    .getMemberGroups(securityEnabledOnly)
    .buildRequest()
    .post();

```