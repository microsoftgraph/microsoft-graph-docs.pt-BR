---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93ad91ef468d5771600afc593238d7149112ad38
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130397"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleDefinitionCollectionPage roleDefinitions = graphClient.roleManagement().directory().roleDefinitions()
    .buildRequest()
    .get();

```