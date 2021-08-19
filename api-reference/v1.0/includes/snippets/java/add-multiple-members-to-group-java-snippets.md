---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3ed3d16c7608fd154e66588c4ba6b6c05cf5b158e250d427a15fc7cb242103a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103005"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.additionalDataManager().put("members@odata.bind", new JsonPrimitive("[  \"https://graph.microsoft.com/v1.0/directoryObjects/{id}\",  \"https://graph.microsoft.com/v1.0/directoryObjects/{id}\",  \"https://graph.microsoft.com/v1.0/directoryObjects/{id}\"]"));

graphClient.groups("{group-id}")
    .buildRequest()
    .patch(group);

```