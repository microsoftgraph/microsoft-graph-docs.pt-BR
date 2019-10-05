---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bdbc7a9c3df877e979ac166a2cbdd4869450bcd8
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402659"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = true;

graphClient.me()
    .getMemberObjects(securityEnabledOnly)
    .buildRequest()
    .post();

```