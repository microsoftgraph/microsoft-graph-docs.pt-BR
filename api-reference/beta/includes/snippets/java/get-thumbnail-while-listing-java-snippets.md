---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a46a279e3ba7fb7910fb4c7670e60df54eba7130
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955791"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage children = graphClient.me().drive().items("{item-id}").children()
    .buildRequest()
    .expand("thumbnails")
    .get();

```