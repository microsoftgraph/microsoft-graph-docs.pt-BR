---
title: Tipo de recurso domainDnsCnameRecord
description: Representa um registro CNAME adicionado ao arquivo de zona DNS de um determinado domínio no locatário.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ecbe5c0dd1d547a6abb116c5152a8d21f0ee3fd8
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760880"
---
# <a name="domaindnscnamerecord-resource-type"></a>Tipo de recurso domainDnsCnameRecord

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um registro CNAME adicionado ao arquivo de zona DNS de um determinado domínio no locatário. Herdada [da entidade DomainDnsRecord.](domaindnsrecord.md)


## <a name="methods"></a>Métodos
Não há suporte para consultas diretas a esse recurso. Consulte o tópico [de domínio](domain.md) para obter informações sobre como consultar registros de serviço de domínio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|canonicalName|Cadeia de Caracteres| O nome canônico do registro CNAME. Usado para configurar o registro CNAME no host DNS. |
|id|Cadeia de caracteres| Identificador exclusivo atribuído a essa entidade. Não anulada, somente leitura|
|isOptional|Boolean| Se for falso, o registro CNAME deverá ser configurado pelo cliente no host DNS para que Microsoft Online Services funcione corretamente com o domínio. Não anulada |
|rótulo|Cadeia de Caracteres| Valor usado ao configurar *o alias/host/nome* do registro CNAME no host DNS. |
|recordType|Cadeia de Caracteres| Tipo de registro DNS. O valor é sempre *CName*. Chave|
|supportedService|Cadeia de Caracteres| Serviço ou recurso do Microsoft Online que tem uma dependência nesse registro CNAME.</br></br>Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*|
|ttl|Int32| Valor a ser usado ao configurar a propriedade time-to-live (ttl) do registro CNAME no host DNS. Não anulada |

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


