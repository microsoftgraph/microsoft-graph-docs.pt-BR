---
title: Tipo de recurso domainDnsRecord
description: Para cada domínio no locatário, talvez seja necessário adicionar registro (s) DNS para o arquivo de zona DNS do domínio para que o domínio que possa ser usado pelo Microsoft Online Services. A entidade **DomainDnsRecord** é usada para apresentar esses registros DNS. Entidade base para entidades DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord e DomainDnsSrvRecord.
localization_priority: Normal
ms.openlocfilehash: 30c5f63f4ecac2c716f7884ccf82fd129125c8b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822341"
---
# <a name="domaindnsrecord-resource-type"></a>Tipo de recurso domainDnsRecord

Para cada domínio no locatário, talvez seja necessário adicionar os registros DNS ao arquivo de zona DNS do domínio para que ele possa ser usado pelo Microsoft Online Services. A entidade **DomainDnsRecord** é usada para apresentar esses registros DNS. A entidade base das entidades [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) e [DomainDnsSrvRecord](domaindnssrvrecord.md).

## <a name="methods"></a>Métodos
Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.|
|isOptional|Booliano| Se for falso, o registro deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio. |
|rótulo|String| O valor usado ao configurar o nome da propriedade do registro DNS no host DNS. |
|recordType|String| Indica que tipo de registro DNS a entidade representa.</br></br>O valor pode ser um dos seguintes: *CName*, *Mx*, *Srv* e *Txt*</br></br>Chave |
|supportedService|String| O Microsoft Online Services ou o recurso que tiver uma dependência neste registro DNS.</br></br>Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*|
|ttl|Int32| O valor a ser usado ao configurar a propriedade time-to-live (ttl) do registro DNS no host DNS. Não anulável |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsRecord"
}-->

```json
{
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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
