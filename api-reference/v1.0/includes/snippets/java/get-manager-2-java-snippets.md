---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e28d17087962649c9f4bd85cdcc945c62d81a85820c9e081fd7baaf4ee9f1639
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407005"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.users("{id|userPrincipalName}").manager()
    .buildRequest()
    .get();

```