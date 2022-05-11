---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6b316830f0d76bc201b4b7e49ec972715701a04
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315719"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    "@odata.type" = "microsoft.graph.samlOrWsFedExternalDomainFederation"
    IssuerUri = "https://contoso.com/issuerUri"
    DisplayName = "contoso display name"
    MetadataExchangeUri = "https://contoso.com/metadataExchangeUri"
    PassiveSignInUri = "https://contoso.com/signin"
    PreferredAuthenticationProtocol = "wsFed"
    Domains = @(
        @{
            "@odata.type" = "microsoft.graph.externalDomainName"
            Id = "contoso.com"
        }
    )
    SigningCertificate = "MIIDADCCAeigAwIBAgIQEX41y8r6"
}

New-MgDirectoryFederationConfiguration -BodyParameter $params

```