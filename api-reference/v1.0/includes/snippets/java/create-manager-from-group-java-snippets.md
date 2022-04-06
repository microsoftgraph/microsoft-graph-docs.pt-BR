---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e907929ec13eb38531c09ef8331223861eb497ef
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759350"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0";

graphClient.users("10f17b99-784c-4526-8747-aec8a3159d6a").manager().reference()
    .buildRequest()
    .put(directoryObject);

```