---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43d1c6f1f1ad8f03f335e024bc020306fc62cad5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978561"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSettingTemplate groupSettingTemplate = graphClient.groupSettingTemplates("{id}")
    .buildRequest()
    .get();

```