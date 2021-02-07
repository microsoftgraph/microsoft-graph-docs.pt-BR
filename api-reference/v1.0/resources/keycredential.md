---
title: Tipo de recurso keyCredential
description: Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço. A **propriedade keyCredentials** do aplicativo e entidades servicePrincipal é uma coleção de **keyCredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 80583c40b61324b2b150c0ab377e4756f227ce39
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135895"
---
# <a name="keycredential-resource-type"></a>Tipo de recurso keyCredential

Namespace: microsoft.graph

Contém uma credencial de chave associada a um aplicativo <!--or a service principal-->. A **propriedade keyCredentials** do [aplicativo](application.md) <!--and [servicePrincipal](serviceprincipal.md)--> é uma coleção de **keyCredential**.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binária| Identificador de chave personalizado |
| displayName | String | Nome amigável da chave. Opcional. |
|endDateTime|DateTimeOffset|A data e a hora em que a credencial expira. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|keyId|Guid|O identificador exclusivo (GUID) da chave.|
|startDateTime|DateTimeOffset|A data e a hora em que a credencial se torna válida. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|type|String|O tipo de credencial de chave; por exemplo, "Simétrico".|
|usage|String|Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; por exemplo, "Verify".|
|chave|Binário| Os dados brutos do certificado em matriz de byte convertidos em cadeia de caracteres Base64; por exemplo, `[System.Convert]::ToBase64String($Cert.GetRawCertData())` . |

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
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

