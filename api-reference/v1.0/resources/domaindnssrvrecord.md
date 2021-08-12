---
title: Tipo de recurso domainDnsSrvRecord
description: Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2322a2425170a930dfaca30224601c01388063dd8d50203c950d1f3b9d5131ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229294"
---
# <a name="domaindnssrvrecord-resource-type"></a>Tipo de recurso domainDnsSrvRecord

Namespace: microsoft.graph

Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdada [da entidade DomainDnsRecord.](domaindnsrecord.md)

## <a name="methods"></a>Métodos
Não há suporte para consultas diretas a esse recurso. Consulte o tópico [de domínio](domain.md) para obter informações sobre como consultar registros de serviço de domínio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Identificador exclusivo atribuído a essa entidade. Não anulada, somente leitura.|
|isOptional|Booliano| Se for falso, o registro SRV deverá ser configurado pelo cliente no host DNS para Microsoft Online Services funcionar corretamente com o domínio. |
|rótulo|Cadeia de caracteres| Valor usado ao configurar a *propriedade name* do registro SRV no host DNS. |
|nameTarget|String| Valor a ser usado ao configurar a *propriedade Target* do registro SRV no host DNS. |
|port|Int32| Valor a ser usado ao configurar a *propriedade de* porta do registro SRV no host DNS. |
|prioridade|Int32| Valor a ser usado ao configurar a *propriedade priority* do registro SRV no host DNS. |
|protocol|Cadeia de caracteres| Valor a ser usado ao configurar a propriedade *de* protocolo do registro SRV no host DNS. |
|recordType|Cadeia de caracteres|  Tipo de registro DNS. O valor é sempre *Srv*. Chave |
|service|Cadeia de caracteres| Valor a ser usado ao configurar a propriedade *de* serviço do registro SRV no host DNS. |
|supportedService|Cadeia de caracteres| Serviço ou recurso do Microsoft Online que tem uma dependência nesse registro SRV.</br></br>Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune* |
|ttl|Int32| Valor a ser usado ao configurar a *propriedade time-to-live (ttl)* do registro SRV no host DNS. Não anulada |
|weight|Int32| Valor a ser usado ao configurar a *propriedade weight* do registro SRV no host DNS. |

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

