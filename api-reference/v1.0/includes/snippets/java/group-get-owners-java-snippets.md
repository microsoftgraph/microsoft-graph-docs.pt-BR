---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5a20237869e5fda3ea689888d72f3b38103f544
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48984079"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage owners = graphClient.groups("{id}").owners()
    .buildRequest()
    .get();

```