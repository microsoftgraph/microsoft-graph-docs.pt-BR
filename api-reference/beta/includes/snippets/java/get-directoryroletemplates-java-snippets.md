---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81bee82f40917b6213176ee3c4599592b302c893
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956244"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryRoleTemplateCollectionPage directoryRoleTemplates = graphClient.directoryRoleTemplates()
    .buildRequest()
    .get();

```