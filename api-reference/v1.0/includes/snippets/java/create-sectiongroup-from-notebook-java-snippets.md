---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7e52cecff789c576fb4f36fb44a33ae932b5dbd23e732fa83f41a0cf396358f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157570"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SectionGroup sectionGroup = new SectionGroup();
sectionGroup.displayName = "Section group name";

graphClient.me().onenote().notebooks("{id}").sectionGroups()
    .buildRequest()
    .post(sectionGroup);

```