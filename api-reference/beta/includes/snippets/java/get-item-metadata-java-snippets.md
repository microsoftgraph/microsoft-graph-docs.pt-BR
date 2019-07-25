---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: efd876d90f7b7f186ed8c0b60ace07d0fc51621f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861134"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.me().drive().root()
    .buildRequest()
    .get();

```