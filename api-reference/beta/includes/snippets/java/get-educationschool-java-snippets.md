---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7cc8644ef50671939a3c2b09e35f077aeb0ea81cfb08ea799e5bc6e9d0aaad0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900236"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchool educationSchool = graphClient.education().schools("10001")
    .buildRequest()
    .get();

```