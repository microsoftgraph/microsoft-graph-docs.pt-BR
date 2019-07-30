---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8487f344990ce55e11b7b9808eaa6bd4fa2d43b9
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35930431"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/directoryObjects/{id}"));

graphClient.applications("{id}").owners().references()
    .buildRequest()
    .post(directoryObject);

```