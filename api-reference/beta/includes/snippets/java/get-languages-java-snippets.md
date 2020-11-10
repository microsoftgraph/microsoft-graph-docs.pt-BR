---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f56b49340feb124e2d885a3073fc728c61027a9e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980758"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ILanguageProficiencyCollectionPage languages = graphClient.me().profile().languages()
    .buildRequest()
    .get();

```