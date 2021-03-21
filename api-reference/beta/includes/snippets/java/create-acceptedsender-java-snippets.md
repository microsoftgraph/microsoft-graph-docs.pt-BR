---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23b1656fa35f7f46de16d6f86e9822aab58012ff
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983617"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "alexd@contoso.com";

graphClient.groups("{id}").acceptedSenders().references()
    .buildRequest()
    .post(directoryObject);

```