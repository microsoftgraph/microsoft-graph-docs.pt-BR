---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa5dab0eb8605403a3959407cf758cf2f2d8f7f1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969383"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/me/drive/items/{item-id}/versions/{version-id}/content", InputStream.class)
    .buildRequest()
    .get();

```