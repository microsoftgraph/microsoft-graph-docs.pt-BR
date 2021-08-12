---
title: Tipo de recurso keyCredential
description: Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço. A **propriedade keyCredentials** das entidades application and servicePrincipal é uma coleção de **keyCredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: ec191064f0dd14cac67279a6802bc57849e4a740c1e1248cba8234e95ce32c96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196954"
---
# <a name="keycredential-resource-type"></a>Tipo de recurso keyCredential

Namespace: microsoft.graph

Contém uma credencial de chave associada a um aplicativo <!--or a service principal-->. A **propriedade keyCredentials** do [aplicativo](application.md) <!--and [servicePrincipal](serviceprincipal.md)--> entity é uma coleção de **keyCredential**.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binário| Identificador de chave personalizada |
| displayName | Cadeia de caracteres | Nome amigável para a chave. Opcional. |
|endDateTime|DateTimeOffset|A data e a hora em que a credencial expira. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|chave|Binário| Os dados brutos do certificado na matriz de byte convertidos na cadeia de caracteres Base64; por exemplo, `[System.Convert]::ToBase64String($Cert.GetRawCertData())` . |
|keyId|Guid|O identificador exclusivo (GUID) da chave.|
|startDateTime|DateTimeOffset|A data e a hora em que a credencial se torna válida. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|tipo|Cadeia de caracteres|O tipo de credencial de chave; por exemplo, `Symmetric` .|
|usage|Cadeia de caracteres|Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; por exemplo, `Verify` .|

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
  "keyId": "Guid",
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

