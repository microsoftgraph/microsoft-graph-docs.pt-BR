---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93fa41353e3ba7dca4be5f86de0c1a3809a55786
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977495"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = graphClient.education().classes("11023")
    .buildRequest()
    .get();

```