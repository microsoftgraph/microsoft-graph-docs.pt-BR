---
title: Tipo de recurso selfSignedCertificate
description: Contém informações sobre a parte pública de um certificado de assinatura.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: luleonpla
ms.openlocfilehash: 09e6ed6adfdfe2803e287bb60496e1b0eeb96a6b
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723679"
---
# <a name="selfsignedcertificate-resource-type"></a>Tipo de recurso selfSignedCertificate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém a parte pública de um certificado de assinatura. É o tipo de retorno da ação [addTokenSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md). Os provedores de serviços usam a parte pública do certificado de assinatura para validar o emissor do token.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo           | Descrição                                                                                                                                                                                                                           |
| ------------------- | -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| customKeyIdentifier | Binária         | Identificador de chave personalizado.                                                                                                                                                                                                                |
| displayName         | String         | O nome amigável da chave.                                                                                                                                                                                                        |
| endDateTime         | DateTimeOffset | A data e a hora em que a credencial expira. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.       |
| keyId               | Guid           | O identificador exclusivo (GUID) da chave.                                                                                                                                                                                             |
| startDateTime       | DateTimeOffset | A data e a hora em que a credencial se torna válida. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| type                | String         | O tipo de credencial de chave. "AsymmetricX509Cert".                                                                                                                                                                                     |
| usage               | String         | Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada. Por exemplo, "Verificar".                                                                                                                                             |
| chave                 | Binário         | O valor da credencial de chave. Deve ser um valor codificado de base-64.                                                                                                                                                                  |
| thumbprint          | String         | O valor de impressão digital da chave.                                                                                                                                                                                                     |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.selfSignedCertificate"
}-->

```json
{
  "@odata.type": "#microsoft.graph.selfSignedCertificate",
  "customKeyIdentifier": "String (Binary)",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "key": "String (Binary)",
  "keyId": "Guid",
  "startDateTime": "String (timestamp)",
  "thumbprint": "String",
  "type": "String",
  "usage": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "selfSignedCertificate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
