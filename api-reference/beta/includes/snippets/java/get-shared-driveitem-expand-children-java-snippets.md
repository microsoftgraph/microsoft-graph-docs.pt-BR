---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c77e3892980158272b66fb121bb8103b5102677c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869840"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.shares("{shareIdOrUrl}").driveItem()
    .buildRequest()
    .expand("children")
    .get();

```