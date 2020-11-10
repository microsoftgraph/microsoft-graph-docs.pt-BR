---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17bb575626d1ca86131b36dbbc659953b74e0138
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979008"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage memberOf = graphClient.contacts("{id}").memberOf()
    .buildRequest()
    .get();

```