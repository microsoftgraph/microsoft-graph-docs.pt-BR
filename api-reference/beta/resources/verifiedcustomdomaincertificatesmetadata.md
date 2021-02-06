---
title: Tipo de recurso verifiedCustomDomainCertificatesMetadata
description: Representa os metadados de cerificate personalizados para um aplicativo local publicado por meio do Proxy de Aplicativo.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: bc0f839d91147f80d41dc48ee53c0f888aa35283
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137589"
---
# <a name="verifiedcustomdomaincertificatesmetadata-resource-type"></a>Tipo de recurso verifiedCustomDomainCertificatesMetadata

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os metadados do certificado de domínio personalizado para o recurso [onPremisesPublishing](onpremisespublishing.md) ao publicar um aplicativo local com o Proxy de Aplicativo. Usar um domínio personalizado permite que você use seu próprio nome de domínio em vez do domínio padrão, msappproxy.net, para seu aplicativo. Para saber mais, confira [domínios personalizados no Proxy de aplicativo do Azure AD.](/azure/active-directory/manage-apps/application-proxy-configure-custom-domain)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|expiryDate|DateTimeOffset| A data de vencimento do certificado de domínio personalizado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. |
|issueDate|DateTimeOffset| A data de emissão do domínio personalizado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. |
|issuerName|String| O nome do emissor do certificado de domínio personalizado. |
|SubjectName|Cadeia de caracteres| O nome da assunto do certificado de domínio personalizado. |
|thumbprint|String| A impressão digital associada ao certificado de domínio personalizado. |

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
