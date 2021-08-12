---
title: tipo de recurso domainDnsUnavailableRecord
description: Indica que serviceConfigurationRecords não pode ser gerado.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ef1a70004e28279f80327b64edb53fd14a0b53f19717ea2f5ed96af5d0039feb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54175312"
---
# <a name="domaindnsunavailablerecord-resource-type"></a>tipo de recurso domainDnsUnavailableRecord

Namespace: microsoft.graph

Ao consultar a propriedade de navegação **serviceConfigurationRecords** para uma entidade [Domain,](domain.md) você pode obter de volta uma ou mais entidades [DomainDnsCnameRecord,](domaindnscnamerecord.md) [DomainDnsMxRecord,](domaindnsmxrecord.md) [DomainDnsSrvRecord](domaindnssrvrecord.md)e/ou [DomainDnsTxtRecord.](domaindnstxtrecord.md) Essas entidades indicam quais registros DNS você deve adicionar ao arquivo de zona do domínio, antes que o domínio possa ser usado por Microsoft Online Services. Quando não é possível gerar essas entidades, uma Entidade DomainDnsUnavailableRecord é retornada. Herdada [da entidade DomainDnsRecord.](domaindnsrecord.md)

## <a name="methods"></a>Métodos
Não há suporte para consultas diretas a esse recurso. Consulte o tópico [de domínio](domain.md) para obter informações sobre como consultar registros de serviço de domínio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|Cadeia de caracteres|Fornece o motivo pelo qual **a entidade DomainDnsUnavailableRecord** é retornada. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "description": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

