---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9378f1ec6536e3741337bda1ce100a0ba8b9706a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864662"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{id}").channels("{id}")
    .buildRequest()
    .delete();

```