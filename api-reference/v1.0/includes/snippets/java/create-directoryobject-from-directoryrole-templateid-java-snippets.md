---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1b39fd472d181efaaa0495cace482bba8ddb66d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976963"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{user-id}";

graphClient.directoryRoles("roleTemplateId={role-templateId}").members().references()
    .buildRequest()
    .post(directoryObject);

```