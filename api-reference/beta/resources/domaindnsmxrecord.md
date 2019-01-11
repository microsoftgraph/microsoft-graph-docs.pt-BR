---
title: Tipo de recurso domainDnsMxRecord
description: Representa um registro MX adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: c6ffa526b359eed6bafa7f38562d5d61c4f4562a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830244"
---
# <a name="domaindnsmxrecord-resource-type"></a>Tipo de recurso domainDnsMxRecord

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um registro MX adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).

## <a name="methods"></a>Métodos
Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.|
|isOptional|Booliano| Se for falso, o registro MX deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio. |
|rótulo|String| O valor usado ao configurar a propriedade *alias/host/name* do registro MX no host DNS. |
|mailExchange|String| O valor usado ao configurar a propriedade *answer/destination/value* do registro MX no host DNS.|
|preference|Int32| O valor usado ao configurar a propriedade *Preference/Priority* do registro MX no host DNS. |
|recordType|String| Tipo do registro DNS. Este valor sempre será *Mx*. Chave |
|supportedService|String| O Microsoft Online Services ou o recurso que tiver uma dependência neste registro MX.</br></br>Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune* |
|ttl|Int32| O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro MX no host DNS. Não anulável |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
