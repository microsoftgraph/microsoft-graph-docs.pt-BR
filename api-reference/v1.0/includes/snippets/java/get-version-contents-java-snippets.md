---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd7c3f589b4d6c3e08117a52d4ec78c4e847b7eb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983295"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/me/drive/items/{item-id}/versions/{version-id}/content", InputStream.class)
    .buildRequest()
    .get();

```