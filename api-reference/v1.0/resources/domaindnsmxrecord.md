---
title: Tipo de recurso domainDnsMxRecord
description: Representa um registro MX adicionado ao arquivo de zona DNS de um determinado domínio no locatário.
author: adimitui
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 41f09764ab4fe2cfde183908db35c99965cce087
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59056106"
---
# <a name="domaindnsmxrecord-resource-type"></a>Tipo de recurso domainDnsMxRecord

Namespace: microsoft.graph

Representa um registro MX adicionado ao arquivo de zona DNS de um determinado domínio no locatário. Herdada [da entidade DomainDnsRecord.](domaindnsrecord.md)

## <a name="methods"></a>Métodos
Não há suporte para consultas diretas a esse recurso. Consulte o tópico [de domínio](domain.md) para obter informações sobre como consultar registros de serviço de domínio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Identificador exclusivo atribuído a essa entidade. Não anulada, somente leitura.|
|isOptional|Boolean| Se for false, o registro MX deve ser configurado pelo cliente no host DNS para Microsoft Online Services operar corretamente com o domínio. |
|rótulo|String| Valor usado ao configurar a *propriedade alias/host/name* do registro MX no host DNS. |
|mailExchange|String| Valor usado ao configurar *a resposta/destino/valor* do registro MX no host DNS.|
|preference|Int32| Valor usado ao configurar a *propriedade Preference/Priority* do registro MX no host DNS. |
|recordType|Cadeia de caracteres| Tipo de registro DNS. O valor é sempre *Mx*. Chave |
|supportedService|String| Serviço ou recurso do Microsoft Online que tem uma dependência nesse registro MX.</br></br>Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune* |
|ttl|Int32| Valor a ser usado ao configurar a *propriedade time-to-live (ttl)* do registro MX no host DNS. Não anulada |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

