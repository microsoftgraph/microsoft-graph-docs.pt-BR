---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 466b3d2be413f497a85f06331c7caf80125b2c26
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885819"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}").versions("{version-id}")
    .restoreVersion()
    .buildRequest()
    .post();

```