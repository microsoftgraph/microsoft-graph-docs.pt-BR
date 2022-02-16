---
title: Tipo de recurso keyCredential
description: Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço. A **propriedade keyCredentials das entidades** application e servicePrincipal é uma coleção **de keyCredential**.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: madansr7
ms.openlocfilehash: 18a96212ca00ad211d1e1848cbfa5e73c552501f
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62853232"
---
# <a name="keycredential-resource-type"></a>Tipo de recurso keyCredential

Namespace: microsoft.graph

Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço. A **propriedade keyCredentials das entidades** [application](application.md) e [servicePrincipal](serviceprincipal.md) é uma coleção **de keyCredential**.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binária| Identificador de chave personalizada |
| displayName | String | Nome amigável para a chave. Opcional. |
|endDateTime|DateTimeOffset|A data e a hora em que a credencial expira. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|chave|Binário| Os dados brutos do certificado na matriz de byte convertidos na cadeia de caracteres Base64. Retornado somente para `$select` um único objeto, ou seja`GET servicePrincipals/{servicePrincipalId}?$select=keyCredentials`, `GET applications/{applicationId}?$select=keyCredentials` ou ; caso contrário, sempre será `null`. |
|keyId|GUID|O identificador exclusivo (GUID) da chave.|
|startDateTime|DateTimeOffset|A data e a hora em que a credencial se torna válida. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|type|String|O tipo de credencial de chave; por exemplo, `Symmetric`, `AsymmetricX509Cert`.|
|usage|String|Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; por exemplo, `Verify`.|

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
  "@odata.type": "#microsoft.graph.keyCredential",
  "customKeyIdentifier": "Binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "key": "Binary",
  "keyId": "GUID",
  "startDateTime": "String (timestamp)",
  "type": "String",
  "usage": "String"
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

