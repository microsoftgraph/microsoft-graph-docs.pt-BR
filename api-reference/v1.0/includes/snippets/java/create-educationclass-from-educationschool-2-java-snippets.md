---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 794dde0fe77e375019166aa45e3dab9cf9b451c23b4dedae75132284b2a0a648
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100261"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("{class-id}").teachers("{teacher-id}")
    .buildRequest()
    .delete();

```