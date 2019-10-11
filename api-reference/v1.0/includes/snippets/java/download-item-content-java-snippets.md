---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02ac68be516df9181f42ae200b7e73fa005fe498
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428748"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Stream stream = graphClient.customRequest("/me/drive/items/{item-id}/content", Stream.class)
    .buildRequest()
    .get();

```