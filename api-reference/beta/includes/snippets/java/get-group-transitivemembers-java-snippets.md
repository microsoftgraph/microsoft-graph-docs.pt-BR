---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af10d94ac8185c41285e956290792ec3aa0d8527
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953889"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage transitiveMembers = graphClient.groups("{id}").transitiveMembers()
    .buildRequest()
    .get();

```