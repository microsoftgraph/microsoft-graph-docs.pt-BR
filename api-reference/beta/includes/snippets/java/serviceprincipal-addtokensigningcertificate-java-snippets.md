---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 604bb0215996f5acdc1f47a487d642de5a563816
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474649"
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