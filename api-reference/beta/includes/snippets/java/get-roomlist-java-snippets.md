---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed5729d1dda94dd0719c153da7558fb814f3d5c8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967417"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Place place = graphClient.places("bldg1@contoso.com")
    .buildRequest()
    .get();

```