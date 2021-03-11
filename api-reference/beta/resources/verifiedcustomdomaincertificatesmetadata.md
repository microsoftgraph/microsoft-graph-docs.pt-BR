---
title: tipo de recurso verifiedCustomDomainCertificatesMetadata
description: Representa os metadados cerificados personalizados para um aplicativo local publicado por meio do Proxy de Aplicativo.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: eab6823bdd3ed6a822cbeabdebf0aedfb654b769
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721429"
---
# <a name="verifiedcustomdomaincertificatesmetadata-resource-type"></a>tipo de recurso verifiedCustomDomainCertificatesMetadata

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os metadados de certificado de domínio personalizados para o [recurso onPremisesPublishing](onpremisespublishing.md) ao publicar um aplicativo local com Proxy de Aplicativo. Usar um domínio personalizado permite que você use seu próprio nome de domínio em vez do domínio padrão, msappproxy.net, para seu aplicativo. Para saber mais, confira [Domínios personalizados no Proxy de Aplicativo do Azure AD.](/azure/active-directory/manage-apps/application-proxy-configure-custom-domain)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|expiryDate|DateTimeOffset| A data de expiração do certificado de domínio personalizado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
|issueDate|DateTimeOffset| A data de emissão do domínio personalizado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
|issuerName|Cadeia de caracteres| O nome do emissor do certificado de domínio personalizado. |
|SubjectName|Cadeia de caracteres| O nome do assunto do certificado de domínio personalizado. |
|thumbprint|Cadeia de caracteres| A impressão digital associada ao certificado de domínio personalizado. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedCustomDomainCertificatesMetadata",
  "baseType": null
}-->

```json
{
  "expiryDate": "String (timestamp)",
  "issueDate": "String (timestamp)",
  "issuerName": "String",
  "subjectName": "String",
  "thumbprint": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedCustomDomainCertificatesMetadata resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
