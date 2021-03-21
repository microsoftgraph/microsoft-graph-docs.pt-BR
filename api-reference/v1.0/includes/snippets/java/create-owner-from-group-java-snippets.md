---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9e1a15e6a0e7d32e8e0da17e4750bbe613de4a9a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976598"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.groups("{id}").owners().references()
    .buildRequest()
    .post(directoryObject);

```