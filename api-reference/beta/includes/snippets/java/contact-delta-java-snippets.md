---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2ac50fad13ecb5205eb6edf277e0a618a91a8b5d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957217"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IContactDeltaCollectionPage delta = graphClient.me().contactFolders("{id}").contacts()
    .delta()
    .buildRequest()
    .select("displayName")
    .get();

```