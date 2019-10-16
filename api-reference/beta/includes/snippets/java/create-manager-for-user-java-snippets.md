---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66428650149b63cd26a5f434255dc92fd57251bc
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544135"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.Id = "{id}";

graphClient.users("{id}").manager().reference()
    .buildRequest()
    .put(directoryObject);

```