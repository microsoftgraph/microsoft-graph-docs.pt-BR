---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99776b8712cf9ab69588fce05d52669721ed21b403afb8398e48cb608dee103c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274634"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{id}")
    .archive(TeamArchiveParameterSet
        .newBuilder()
        .withShouldSetSpoSiteReadOnlyForMembers(null)
        .build())
    .buildRequest()
    .post();

```