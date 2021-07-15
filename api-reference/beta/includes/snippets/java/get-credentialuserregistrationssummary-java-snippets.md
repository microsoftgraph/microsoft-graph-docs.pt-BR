---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17bb09627499c668a8730f0e25f399a538092e31
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440020"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CredentialUserRegistrationsSummary credentialUserRegistrationsSummary = graphClient.tenantRelationships().managedTenants().credentialUserRegistrationsSummaries("{credentialUserRegistrationsSummaryId}")
    .buildRequest()
    .get();

```