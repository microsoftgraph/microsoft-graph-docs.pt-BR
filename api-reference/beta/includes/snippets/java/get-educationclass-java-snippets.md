---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0aa4da45f5fef4fb7fd980ab6af4ebe1c3bbaa4d7fbff1cc4caa2e70f83ca539
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216594"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = graphClient.education().classes("11023")
    .buildRequest()
    .get();

```