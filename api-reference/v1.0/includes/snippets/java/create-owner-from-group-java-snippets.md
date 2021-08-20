---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d337d5383c666dc9b9ddd60fe50b41039f3f60b16c5a48480ec5f3a2661764c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375970"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.groups("{id}").owners().references()
    .buildRequest()
    .post(directoryObject);

```