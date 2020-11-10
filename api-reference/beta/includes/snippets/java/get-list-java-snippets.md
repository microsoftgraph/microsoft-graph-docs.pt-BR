---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99fdfcaef3034c21d847411d930cb0a91f2f3633
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969742"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

List list = graphClient.sites("{site-id}").lists("{list-title}")
    .buildRequest()
    .get();

```