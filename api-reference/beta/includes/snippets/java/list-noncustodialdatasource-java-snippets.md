---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af3d306209dfb55affe514fe701024f718ab26bc2c61d548da71dbed59cc9dbc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156327"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NoncustodialDataSourceCollectionPage noncustodialDataSources = graphClient.compliance().ediscovery().cases("5b840b94-f821-4c4a-8cad-3a90062bf51a").noncustodialDataSources()
    .buildRequest()
    .get();

```