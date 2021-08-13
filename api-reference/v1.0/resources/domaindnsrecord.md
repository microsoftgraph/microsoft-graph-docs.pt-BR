---
title: Tipo de recurso domainDnsRecord
description: A entidade DomainDnsRecord é usada para apresentar registros DNS.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: cffbc9210d16027a804eb7c48192b05f1fd2b13f1df7a2f4c377a0bc0faf6327
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141767"
---
# <a name="domaindnsrecord-resource-type"></a>Tipo de recurso domainDnsRecord

Namespace: microsoft.graph

Para cada domínio no locatário, talvez seja necessário adicionar registros DNS ao arquivo de zona DNS do domínio antes que o domínio possa ser usado por Microsoft Online Services. A **entidade DomainDnsRecord** é usada para apresentar esses registros DNS. Entidade base [para entidades DomainDnsCnameRecord,](domaindnscnamerecord.md) [DomainDnsMxRecord,](domaindnsmxrecord.md) [DomainDnsSrvRecord](domaindnssrvrecord.md) e [DomainDnsTxtRecord.](domaindnstxtrecord.md)

## <a name="methods"></a>Métodos
Não há suporte para consultas diretas a esse recurso. Consulte o tópico [de domínio](domain.md) para obter informações sobre como consultar registros de serviço de domínio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Identificador exclusivo atribuído a essa entidade. Não anulada, somente leitura.|
|isOptional|Booliano| Se for falso, esse registro deverá ser configurado pelo cliente no host DNS para que Microsoft Online Services funcione corretamente com o domínio. |
|rótulo|Cadeia de caracteres| Valor usado ao configurar o nome do registro DNS no host DNS. |
|recordType|Cadeia de caracteres| Indica que tipo de registro DNS essa entidade representa.</br></br>O valor pode ser um dos seguintes: *CName*, *Mx,* *Srv,* *Txt*</br></br>Chave |
|supportedService|String| Serviço ou recurso do Microsoft Online que tem uma dependência nesse registro DNS.</br></br>Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*|
|ttl|Int32| Valor a ser usado ao configurar a propriedade time-to-live (ttl) do registro DNS no host DNS. Não anulada |

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

