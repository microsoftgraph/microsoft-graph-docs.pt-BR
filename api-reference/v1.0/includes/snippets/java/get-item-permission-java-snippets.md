---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c234985c7446ac3ffa4a5699ecbccb0076a1bea7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886491"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Permission permission = graphClient.me().drive().items("{item-id}").permissions("{perm-id}")
    .buildRequest()
    .get();

```