---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38383c02d635b1888860903995d41b06a67bae5d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979979"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InferenceClassificationOverrideCollectionPage overrides = graphClient.me().inferenceClassification().overrides()
    .buildRequest()
    .get();

```