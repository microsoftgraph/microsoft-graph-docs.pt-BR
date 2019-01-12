---
title: Tipo de recurso domainDnsUnavailableRecord
description: Quando você consulta para a propriedade de navegação **serviceConfigurationRecords** para uma entidade de domínio, você pode obter novamente uma ou mais entidades de DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord e/ou DomainDnsTxtRecord. Essas entidades indicam quais registros DNS, você deve adicionar o arquivo de zona do domínio, antes que o domínio pode ser usado pelo Microsoft Online Services. Quando não é possível gerar tais entidades, uma entidade DomainDnsUnavailableRecord é retornada em vez disso. Herdado de entidade DomainDnsRecord.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99da0448d75375b84bb37c05102c1f702c222a25
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982789"
---
# <a name="domaindnsunavailablerecord-resource-type"></a>Tipo de recurso domainDnsUnavailableRecord

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Ao consultar a propriedade de navegação **serviceConfigurationRecords** de uma entidade [Domain](domain.md), você pode receber novamente uma ou mais entidades [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) e/ou [DomainDnsTxtRecord](domaindnstxtrecord.md). Essas entidades indicam quais registros DNS você deve adicionar ao arquivo de zona do domínio antes que ele possa ser usado pelo Microsoft Online Services. Quando não for possível gerar essas entidades, uma entidade DomainDnsUnavailableRecord será retornada. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).

## <a name="methods"></a>Métodos
Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|String|Fornece a razão pela qual a entidade **DomainDnsUnavailableRecord** será retornada. |

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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
