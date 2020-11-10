---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 806a6bb8aaa88252c84d839ad5e28462bc5a43be
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962853"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage registeredUsers = graphClient.devices("{id}").registeredUsers()
    .buildRequest()
    .get();

```