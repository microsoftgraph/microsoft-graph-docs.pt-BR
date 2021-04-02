---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5813f4f3821573616738498ea6871ea1ddeef59
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507187"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstance accessReviewInstance = graphClient.identityGovernance().accessReviews().definitions("6af553ce-104d-4842-ab5f-67d7b556e9dd").instances("9ea56d3c-8746-4cdf-9ccc-c7fe1a267c24")
    .buildRequest()
    .get();

```