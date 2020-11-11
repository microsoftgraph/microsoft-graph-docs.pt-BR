---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 394b97f9ff90eba7963b71ae05fc64ca62f9b781
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983653"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "alexd@contoso.com";

graphClient.groups("{id}").rejectedSenders().references()
    .buildRequest()
    .post(directoryObject);

```