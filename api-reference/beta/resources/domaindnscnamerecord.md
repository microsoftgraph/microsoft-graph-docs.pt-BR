---
title: Tipo de recurso domainDnsCnameRecord
description: Representa um registro CNAME adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f270075556843625d1ec408f06be8ed4a065c831
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516732"
---
# <a name="domaindnscnamerecord-resource-type"></a>Tipo de recurso domainDnsCnameRecord

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um registro CNAME adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).


## <a name="methods"></a>Métodos
Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|canonicalName|String| O nome canônico do registro CNAME. Usado para configurar o registro CNAME no host DNS. |
|id|String| Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura|
|isOptional|Booliano| Se for falso, o registro CNAME deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio. Não anulável |
|rótulo|String| O valor usado ao configurar a propriedade *alias/host/name* do registro CNAME no host DNS. |
|recordType|String| Tipo do registro DNS. Este valor sempre será *CName*. Chave|
|supportedService|String| O Microsoft Online Services ou o recurso que tiver uma dependência neste registro CNAME.</br></br>Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*|
|ttl|Int32| O valor a ser usado ao configurar a propriedade time-to-live (ttl) do registro CNAME no host DNS. Não anulável |

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsCnameRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/domaindnscnamerecord.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
