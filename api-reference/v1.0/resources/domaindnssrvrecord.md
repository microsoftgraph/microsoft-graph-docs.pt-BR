---
title: Tipo de recurso domainDnsSrvRecord
description: Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade DomainDnsRecord.
ms.openlocfilehash: 1fd1123866d1674aec167de8bec8ef9a45be8d99
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005244"
---
# <a name="domaindnssrvrecord-resource-type"></a>Tipo de recurso domainDnsSrvRecord

Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).

## <a name="methods"></a>Métodos
Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.|
|isOptional|Booliano| Se for falso, o registro SRV deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio. |
|rótulo|String| O valor usado ao configurar a propriedade *name* do registro SRV no host DNS. |
|nameTarget|String| O valor a ser usado ao configurar a propriedade *Target* do registro SRV no host DNS. |
|porta|Int32| O valor a ser usado ao configurar a propriedade *port* do registro SRV no host DNS. |
|prioridade|Int32| O valor a ser usado ao configurar a propriedade *priority* do registro SRV no host DNS. |
|protocolo|String| O valor a ser usado ao configurar a propriedade *protocol* do registro SRV no host DNS. |
|recordType|String|  Tipo do registro DNS. Este valor sempre será *Srv*. Chave |
|service|String| O valor a ser usado ao configurar a propriedade *service* do registro SRV no host DNS. |
|supportedService|String| O Microsoft Online Services ou o recurso que tiver uma dependência neste registro SRV.</br></br>Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune* |
|ttl|Int32| O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro SRV no host DNS. Não anulável |
|weight|Int32| O valor a ser usado ao configurar a propriedade *weight* do registro SRV no host DNS. |

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