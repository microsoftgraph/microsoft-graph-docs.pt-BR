---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bddaf71db37b9a50569de73fe24d3959f5967130
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209580"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TagCollectionWithReferencesPage childTags = graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").tags("e54b3f535b434a9a8743b84e34c00504").childTags()
    .buildRequest()
    .get();

```