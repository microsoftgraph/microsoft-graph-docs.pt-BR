---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee3cd8aa80210c04e9df4fd93eae5017ec962737
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983123"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.users("{id}").manager().reference()
    .buildRequest()
    .put(directoryObject);

```