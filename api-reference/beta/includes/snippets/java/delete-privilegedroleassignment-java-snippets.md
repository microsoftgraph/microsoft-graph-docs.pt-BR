---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 013c7920b06f0d0d6d5ba54277df511efab3d3a087ce14e664b41bf1d53b813f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159198"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.privilegedRoleAssignments("{id}")
    .buildRequest()
    .delete();

```