---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b741bd2026689f96f86d51f6b58e6581070cf6f98198af845f2fb5bb2fe546dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099613"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationTemplate synchronizationTemplate = new SynchronizationTemplate();
synchronizationTemplate.id = "SCIM-Test1";
synchronizationTemplate.applicationId = UUID.fromString("{id}");
synchronizationTemplate.factoryTag = "CustomSCIM";

graphClient.applications("{id}").synchronization().templates()
    .buildRequest()
    .post(synchronizationTemplate);

```