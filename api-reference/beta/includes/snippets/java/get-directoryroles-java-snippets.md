---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 759636201348944f1c010ce1e06fd7b2623a36e582db3a1a80c082a33e3e8141
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217321"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRoleCollectionPage directoryRoles = graphClient.directoryRoles()
    .buildRequest()
    .get();

```