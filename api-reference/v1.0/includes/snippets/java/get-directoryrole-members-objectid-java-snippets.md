---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64587d1cc09e72177621c9130c1ab942a600137f
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524558"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage members = graphClient.directoryRoles("23f3b4b4-8a29-4420-8052-e4950273bbda").members()
    .buildRequest()
    .get();

```