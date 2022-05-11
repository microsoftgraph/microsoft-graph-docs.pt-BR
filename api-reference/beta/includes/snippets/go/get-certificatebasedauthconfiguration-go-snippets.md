---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 503241c9350c651038926f4aaf90b8f189461fd1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323918"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

organizationId := "organization-id"
certificateBasedAuthConfigurationId := "certificateBasedAuthConfiguration-id"
result, err := graphClient.OrganizationById(&organizationId).CertificateBasedAuthConfigurationById(&certificateBasedAuthConfigurationId).Get()


```