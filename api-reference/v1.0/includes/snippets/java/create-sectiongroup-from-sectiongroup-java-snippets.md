---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 09764287cd3c627f5144137e8a7fd5f7fabac8b4dbc817958975358560e4a20e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216464"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SectionGroup sectionGroup = new SectionGroup();
sectionGroup.displayName = "Section group name";

graphClient.me().onenote().sectionGroups("{id}").sectionGroups()
    .buildRequest()
    .post(sectionGroup);

```