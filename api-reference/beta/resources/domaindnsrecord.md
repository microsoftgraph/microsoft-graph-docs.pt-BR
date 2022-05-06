---
title: Tipo de recurso domainDnsRecord
description: A entidade domainDnsRecord é usada para apresentar registros DNS.
ms.localizationpriority: medium
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 327a07fcbca5c9c02bca90e46ceff9454c3267f3
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246556"
---
# <a name="domaindnsrecord-resource-type"></a>Tipo de recurso domainDnsRecord

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Para cada [domínio](domain.md) no locatário, talvez seja necessário adicionar registros DNS ao arquivo de zona DNS do domínio antes que o domínio possa ser usado pelo Microsoft Online Services. A **entidade domainDnsRecord** é usada para apresentar esses registros DNS. Esse tipo de recurso é a entidade base para os seguintes recursos:
+ [domainDnsCnameRecord](domaindnscnamerecord.md)
+ [domainDnsMxRecord](domaindnsmxrecord.md)
+ [domainDnsSrvRecord](domaindnssrvrecord.md)
+ [domainDnsTxtRecord](domaindnstxtrecord.md)
+ [domainDnsUnavailableRecord](domaindnsunavailablerecord.md)

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Identificador exclusivo atribuído a essa entidade. Não anulável, somente leitura.|
|Isoptional|Booliano| Se for false, esse registro deverá ser configurado pelo cliente no host DNS para que o Microsoft Online Services opere corretamente com o domínio. |
|rótulo|Cadeia de caracteres| Valor usado ao configurar o nome do registro DNS no host DNS. |
|recordType|Cadeia de caracteres| Indica o tipo de registro DNS que essa entidade representa.</br></br>O valor pode ser um dos seguintes: `CName`, , `Mx``Srv`, `Txt`. |
|supportedService|Cadeia de caracteres| Serviço Online da Microsoft ou recurso que tem uma dependência nesse registro DNS.</br></br>Pode ser um dos seguintes valores: , , , , `EmailInternalRelayOnly`, `OfficeCommunicationsOnline`, , `SharePointDefaultDomain`, `FullRedelegation`, `SharePointPublic`, `OrgIdAuthentication`, , `Yammer`, , `Intune`. `Sharepoint``Email``null`|
|Ttl|Int32| Valor a ser usado ao configurar a propriedade ttl (vida útil) do registro DNS no host DNS. Não anulável. |

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


