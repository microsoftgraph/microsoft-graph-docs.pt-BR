---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a2d9148f777c72e5d7888f3148857f89f019bd87
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210890"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.devices("{id}").registeredUsers().references()
    .buildRequest()
    .post(directoryObject);

```