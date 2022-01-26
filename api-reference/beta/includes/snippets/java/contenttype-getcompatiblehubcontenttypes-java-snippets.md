---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee9e3058c50a9579e65d93bd67037288eea49842
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225230"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContentTypeGetCompatibleHubContentTypesCollectionPage getCompatibleHubContentTypes = graphClient.sites("{siteId}").lists("{listId}").contentTypes()
    .getCompatibleHubContentTypes()
    .buildRequest()
    .get();

```