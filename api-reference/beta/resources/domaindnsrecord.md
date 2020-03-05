---
title: tipo de recurso domainDnsRecord
description: Para cada domínio no locatário, talvez seja necessário adicionar registros DNS ao arquivo de zona DNS do domínio antes que o domínio possa ser usado pelo Microsoft Online Services. A entidade **DomainDnsRecord** é usada para apresentar esses registros DNS. Entidade base para entidades DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord e DomainDnsTxtRecord.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4eb36c4d57826dab8e2da83eeab2bfaf577008c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42506292"
---
# <a name="domaindnsrecord-resource-type"></a>tipo de recurso domainDnsRecord

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Para cada domínio no locatário, talvez seja necessário adicionar registros DNS ao arquivo de zona DNS do domínio antes que o domínio possa ser usado pelo Microsoft Online Services. A entidade **DomainDnsRecord** é usada para apresentar esses registros DNS. Entidade base para entidades [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) e [DomainDnsTxtRecord](domaindnstxtrecord.md) .

## <a name="methods"></a>Métodos
Não há suporte para consultas diretas a esse recurso. Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Identificador exclusivo atribuído a esta entidade. Não anulável, somente leitura.|
|IsOptional|Boolean| Se for false, esse registro deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio. |
|rótulo|String| O valor usado ao configurar o nome do registro DNS no host DNS. |
|recordType|String| Indica o tipo de registro DNS que esta entidade representa.</br></br>O valor pode ser um dos seguintes: *CNAME*, *MX*, *SRV*, *txt*</br></br>Chave |
|supportedService|String| O Microsoft Online Services ou o recurso que tem uma dependência neste registro DNS.</br></br>Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*|
|TTL|Int32| O valor a ser usado ao configurar a propriedade time-to-Live (TTL) do registro DNS no host DNS. Não anulável |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
