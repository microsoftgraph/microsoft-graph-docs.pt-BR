---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f84c3c0b1fa32ac216d912592a3d6a71033e7d19
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225169"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewReviewerCollectionPage contactedReviewers = graphClient.identityGovernance().accessReviews().definitions("2dca8959-b716-4b4c-a93d-a535c01eb6e0").instances("8d035c9d-798d-47fa-beb4-f986a4b8126f").contactedReviewers()
    .buildRequest()
    .get();

```