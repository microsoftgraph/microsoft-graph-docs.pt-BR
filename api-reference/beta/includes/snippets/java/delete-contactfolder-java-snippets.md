---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 200f3ceee704ada36629ef9f9becb11aed314e90
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863320"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().contactFolders("{id}")
    .buildRequest()
    .delete();

```