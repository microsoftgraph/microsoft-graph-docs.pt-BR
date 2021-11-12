---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 203a06be45604c3d437be45f1cb02ba952d8826bed67d7b3a8811ebd0ae4f896
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158760"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskGroup outlookTaskGroup = new OutlookTaskGroup();
outlookTaskGroup.name = "Personal Tasks";

graphClient.me().outlook().taskGroups("AAMkADIyAAAhrbe-AAA=")
    .buildRequest()
    .patch(outlookTaskGroup);

```