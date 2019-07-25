---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb40565214b0ce0b662db5d63c75738d9c756acd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893747"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOneDriveActivityUserDetail('D7')
    .buildRequest()
    .get();

```