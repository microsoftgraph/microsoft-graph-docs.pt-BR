---
title: tipo de recurso de keyCredential
description: Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço. A propriedade **keyCredentials** das entidades que aplicativo e servicePrincipal é uma coleção de **keyCredential**.
localization_priority: Normal
ms.openlocfilehash: 0319568dad271f13b396d2f75a71839e85c96c40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851559"
---
# <a name="keycredential-resource-type"></a>tipo de recurso de keyCredential

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço. A propriedade **keyCredentials** das entidades que [aplicativo](application.md) e [servicePrincipal](serviceprincipal.md) é uma coleção de **keyCredential**.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binária| Identificador de chave personalizado |
|endDateTime|DateTimeOffset|A data e hora em que a credencial de expiração. O tipo de carimbo de hora representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|keyId|Guid|O identificador exclusivo (GUID) para a chave.|
|startDateTime|DateTimeOffset|A data e hora em que a credencial torna-se válido. O tipo de carimbo de hora representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|type|Cadeia de caracteres|O tipo de credencial de chave; Por exemplo, "Simétrico".|
|uso|Cadeia de caracteres|Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; Por exemplo, "Verificar".|
|chave|Binário|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
