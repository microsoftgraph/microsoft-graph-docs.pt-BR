---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65ed1f2b6b22cdb194ef718598eb9c6e49943941
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969972"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAddress itemAddress = graphClient.me().profile().addresses("{id}")
    .buildRequest()
    .get();

```