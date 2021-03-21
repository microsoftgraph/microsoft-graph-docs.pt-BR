---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 894948cae15639ea79bc31a4ec35fc9e12744798
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976238"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.additionalDataManager().put("members@odata.bind", new JsonPrimitive("[  \"https://graph.microsoft.com/v1.0/directoryObjects/{id}\",  \"https://graph.microsoft.com/v1.0/directoryObjects/{id}\",  \"https://graph.microsoft.com/v1.0/directoryObjects/{id}\"]"));

graphClient.groups("{group-id}")
    .buildRequest()
    .patch(group);

```