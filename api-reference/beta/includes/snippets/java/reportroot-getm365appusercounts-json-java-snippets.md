---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 939e49e47958630b7cedbcebf01291ca4ae3f510
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975952"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/reports/getM365AppUserCounts(period='D7')/content", InputStream.class)
    .buildRequest()
    .get();

```