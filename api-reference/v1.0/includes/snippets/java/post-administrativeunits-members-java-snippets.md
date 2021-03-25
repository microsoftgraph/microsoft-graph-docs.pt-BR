---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59e885a209608f0a0164958d4aa882ac890ba3b6
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202134"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.directory().administrativeUnits("{id}").members().references()
    .buildRequest()
    .post(directoryObject);

```