---
title: Tipo de recurso domainDnsRecord
description: A entidade DomainDnsRecord é usada para apresentar registros DNS.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ba4955c670548b3670dc90a574bc1b4fd8a11c58
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135104"
---
# <a name="domaindnsrecord-resource-type"></a>Tipo de recurso domainDnsRecord

Namespace: microsoft.graph

Para cada domínio no locatário, talvez seja necessário adicionar registros DNS ao arquivo de zona DNS do domínio antes que o domínio possa ser usado pelo Microsoft Online Services. A **entidade DomainDnsRecord** é usada para apresentar esses registros DNS. Entidade base [para entidades DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) e [domainDnsTxtRecord.](domaindnstxtrecord.md)

## <a name="methods"></a>Methods
Não há suporte para consultas diretas a esse recurso. Consulte o tópico [de domínio](domain.md) para obter informações sobre como consultar registros de serviço de domínio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Identificador exclusivo atribuído a essa entidade. Não anulavel, somente leitura.|
|isOptional|Booliano| Se for falso, esse registro deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para operar corretamente com o domínio. |
|rótulo|String| Valor usado ao configurar o nome do registro DNS no host DNS. |
|recordType|String| Indica o tipo de registro DNS que essa entidade representa.</br></br>O valor pode ser um dos seguintes: *CName*, *Mx*, *Srv*, *Txt*</br></br>Chave |
|supportedService|String| Microsoft Online Service ou recurso que tem uma dependência nesse registro DNS.</br></br>Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*|
|ttl|Int32| Valor a ser usado ao configurar a propriedade time-to-live (ttl) do registro DNS no host DNS. Não anulavel |

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

