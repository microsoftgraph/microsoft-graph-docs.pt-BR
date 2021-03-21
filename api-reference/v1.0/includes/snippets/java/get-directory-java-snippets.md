---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 89871ae93d300e5f07fe8b3265d818f3944ce81c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976469"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directory().deletedItems("{object-id}")
    .buildRequest()
    .get();

```