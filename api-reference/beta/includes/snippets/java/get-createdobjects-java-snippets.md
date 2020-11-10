---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de02d6ce746ae6289927d2765f8a6ca294f37adb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971742"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage createdObjects = graphClient.me().createdObjects()
    .buildRequest()
    .get();

```