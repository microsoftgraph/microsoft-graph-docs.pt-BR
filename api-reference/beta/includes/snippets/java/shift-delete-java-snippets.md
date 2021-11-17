---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c766044541e44b7dd4115f11272b4b2749fa1d0329c7dbd27bc245977d24fb66
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101693"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamId}").schedule().shifts("{shiftId}")
    .buildRequest()
    .delete();

```