---
title: tipo de recurso domainDnsUnavailableRecord
description: Ao consultar a propriedade de navegação **serviceConfigurationRecords** para uma entidade de domínio, você pode obter uma ou mais entidades DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord e/ou DomainDnsTxtRecord. Essas entidades indicam quais registros DNS você deve adicionar ao arquivo de zona do domínio, antes que o domínio possa ser usado pelo Microsoft Online Services. Quando não for possível gerar essas entidades, uma entidade DomainDnsUnavailableRecord será retornada. Herdado de entidade DomainDnsRecord.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5f033c39c9cf8dc11c2a41b0cedb0b8de5ce7736
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562766"
---
# <a name="domaindnsunavailablerecord-resource-type"></a>tipo de recurso domainDnsUnavailableRecord

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ao consultar a propriedade de navegação **serviceConfigurationRecords** para uma entidade de [domínio](domain.md) , você pode obter uma ou mais [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md)e/ou [ Entidades DomainDnsTxtRecord](domaindnstxtrecord.md) . Essas entidades indicam quais registros DNS você deve adicionar ao arquivo de zona do domínio, antes que o domínio possa ser usado pelo Microsoft Online Services. Quando não for possível gerar essas entidades, uma entidade DomainDnsUnavailableRecord será retornada. Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .

## <a name="methods"></a>Métodos
Não há suporte para consultas diretas a esse recurso. Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|String|Fornece o motivo pelo qual a entidade **DomainDnsUnavailableRecord** é retornada. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "canonicalName": "String",
  "description": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
