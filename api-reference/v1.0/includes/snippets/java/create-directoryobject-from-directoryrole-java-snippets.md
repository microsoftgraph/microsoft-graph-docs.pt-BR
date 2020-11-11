---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 906ed729439f8020c9d571cb298afaec13438eb2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983131"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.directoryRoles("{id}").members().references()
    .buildRequest()
    .post(directoryObject);

```