---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 315fff8c96828b96bfa0bf2a18a3755323e79c67
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209493"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage ownedObjects = graphClient.me().ownedObjects()
    .buildRequest()
    .get();

```