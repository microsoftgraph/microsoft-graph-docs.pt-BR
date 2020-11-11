---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5177e032000f7a17da6e5551bf3bb6dcdd78647d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983359"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage createdObjects = graphClient.servicePrincipals("{id}").createdObjects()
    .buildRequest()
    .get();

```