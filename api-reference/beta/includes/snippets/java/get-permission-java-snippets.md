---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72583bb29f8c18a83d7d455ba88104ffc596f91375aaab9329dc1d9a46537fcb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159187"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Permission permission = graphClient.sites("{sitesId}").permissions("{permissionId}")
    .buildRequest()
    .get();

```