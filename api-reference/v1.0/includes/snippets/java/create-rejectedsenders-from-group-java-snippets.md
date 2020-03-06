---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 68ee2ad94bbba0e5af477553eff7fc69316ba156
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544133"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.Id = "alexd@contoso.com";

graphClient.groups("{id}").rejectedSenders().references()
    .buildRequest()
    .post(directoryObject);

```