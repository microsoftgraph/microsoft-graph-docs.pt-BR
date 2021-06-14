---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 655ba97e2735096988031d4478ad0474e8bae81a
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871577"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClassCollectionWithReferencesPage taughtClasses = graphClient.education().users("{educationUserId}").taughtClasses()
    .buildRequest()
    .get();

```