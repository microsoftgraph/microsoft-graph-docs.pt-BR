---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2c11b8021dbb222f38109c66ad4650ec84dd81de
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955792"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IThumbnailSetCollectionPage thumbnails = graphClient.me().drive().items("{item-id}").thumbnails()
    .buildRequest()
    .get();

```