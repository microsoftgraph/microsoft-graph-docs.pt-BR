---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 305e8f0d9cc853867eede6e8b5a729f62ae9d77d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961922"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.applications("{id}").owners().references()
    .buildRequest()
    .post(directoryObject);

```