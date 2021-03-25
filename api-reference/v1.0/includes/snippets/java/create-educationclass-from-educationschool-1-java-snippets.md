---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3e99a9b013b52e3835bad1f8c38432de5c2c60fc
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208371"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("{class-id}").members("{member-id}")
    .buildRequest()
    .delete();

```