---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db87efbc70b1d5e4e2587358f79469a6da106e5f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983832"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directoryRoles("roleTemplateId={role-templateId}").members("{user-id}").reference()
    .buildRequest()
    .delete();

```