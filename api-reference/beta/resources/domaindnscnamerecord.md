---
title: tipo de recurso domainDnsCnameRecord
description: Representa um registro CNAME adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado de entidade DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a76818c23890a011a4607629b16122a767126178
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012755"
---
# <a name="domaindnscnamerecord-resource-type"></a>tipo de recurso domainDnsCnameRecord

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um registro CNAME adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .


## <a name="methods"></a>Métodos
Não há suporte para consultas diretas a esse recurso. Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|canônicaname|String| O nome canônico do registro CNAME. Usado para configurar o registro CNAME no host DNS. |
|id|String| Identificador exclusivo atribuído a esta entidade. Não anulável, somente leitura|
|IsOptional|Booliano| Se for falso, o registro CNAME deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio. Não anulável |
|rótulo|String| O valor usado ao configurar o *alias/host/nome* do registro CNAME no host DNS. |
|recordType|String| Tipo de registro DNS. O valor é sempre *CNAME*. Chave|
|supportedService|String| O Microsoft Online Services ou o recurso que tem uma dependência neste registro CNAME.</br></br>Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic *, *OrgIdAuthentication*, *Yammer*, *Intune*|
|TTL|Int32| O valor a ser usado ao configurar a propriedade TTL (time-to-Live) do registro CNAME no host DNS. Não anulável |

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
  "suppressions": []
}
-->
