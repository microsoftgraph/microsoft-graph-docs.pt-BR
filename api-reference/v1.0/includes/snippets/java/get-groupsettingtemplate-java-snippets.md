---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 920ed50a2dce17cba390592e27553cbb04f46cb4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889381"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSettingTemplate groupSettingTemplate = graphClient.groupSettingTemplates("{id}")
    .buildRequest()
    .get();

```