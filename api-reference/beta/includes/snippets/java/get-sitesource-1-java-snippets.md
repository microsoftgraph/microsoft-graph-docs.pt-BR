---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 280bdd5805f69abf00935067752b0e06e317d023d74f01803217d12b2d7bb6fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159682"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteSourceCollectionPage siteSources = graphClient.compliance().ediscovery().cases("4c8f8f70-7785-4bd4-b296-c98376a2c5e1").custodians("2192ca408ea2410eba3bec8ae873be6b").siteSources()
    .buildRequest()
    .get();

```