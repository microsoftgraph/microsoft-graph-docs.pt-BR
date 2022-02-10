---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 604bb0215996f5acdc1f47a487d642de5a563816
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519212"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "CN=customDisplayName";

OffsetDateTime endDateTime = OffsetDateTimeSerializer.deserialize("01/25/2024 00:00:00");

graphClient.servicePrincipals("004375c5-6e2e-4dec-95e3-626838cb9f80")
    .addTokenSigningCertificate(ServicePrincipalAddTokenSigningCertificateParameterSet
        .newBuilder()
        .withDisplayName(displayName)
        .withEndDateTime(endDateTime)
        .build())
    .buildRequest()
    .post();

```