---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b20d4b5c7272503165d601e0a82ed757a57da59a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544146"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.Id = "alexd@contoso.com";

graphClient.groups("{id}").acceptedSenders().references()
    .buildRequest()
    .post(directoryObject);

```