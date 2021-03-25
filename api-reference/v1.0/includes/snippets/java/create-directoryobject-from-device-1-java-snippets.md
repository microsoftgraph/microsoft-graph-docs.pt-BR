---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 627c615c1d1ea6929469b4c5bbd0a575a2f010f4
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210529"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.devices("{id}").registeredOwners().references()
    .buildRequest()
    .post(directoryObject);

```