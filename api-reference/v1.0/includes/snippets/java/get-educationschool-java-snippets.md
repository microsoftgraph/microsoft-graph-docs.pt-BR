---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 450eb79079d56e7a788cf10cb87afab6761d3adb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968182"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchool educationSchool = graphClient.education().schools("{school-id}")
    .buildRequest()
    .get();

```