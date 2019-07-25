---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0727804d9b54e1dfb934744943da841d9bfbaf73
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893107"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().mailFolders("{id}")
    .buildRequest()
    .delete();

```