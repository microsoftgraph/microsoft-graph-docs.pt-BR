---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: adebae49c347841775d39317c12070c1b91eae18
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286493"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).CertificateBasedAuthConfiguration().Get(nil)


```