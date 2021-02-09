---
title: Tipo de recurso securityAction
description: Executar uma ação imediata proteger contra ameaças usando a entidade securityActionde Segurança do Microsoft Graph. Quando um analista de segurança descobre um indicador novo, como um arquivo mal-intencionado, URL, domínio ou endereço IP, a proteção pode ser habilitada instantaneamente em suas soluções de segurança da Microsoft. Usar uma ação específica do provedor, ver todas as ações executadas e cancelar uma ação, se necessário. Experimente as ações de segurança com o ATP do Windows Defender (em breve) para bloquear as atividades mal-intencionados seus pontos de extremidade do Windows usando as propriedades vistas nos alertas ou identificadas durante as investigações.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 9bd20ddb5a228cf6764dc2ecf6ff770218ca916a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159434"
---
# <a name="securityaction-resource-type"></a>Tipo de recurso securityAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Executar uma ação imediata proteger contra ameaças usando a entidade securityActionde Segurança do Microsoft Graph. Quando um analista de segurança descobre um indicador novo, como um arquivo mal-intencionado, URL, domínio ou endereço IP, a proteção pode ser habilitada instantaneamente em suas soluções de segurança da Microsoft. Usar uma ação específica do provedor, ver todas as ações executadas e cancelar uma ação, se necessário. Experimente as ações de segurança com o [ATP do Windows Defender](/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection)para bloquear as atividades mal-intencionados em seus pontos de extremidade do Windows usando as propriedades vistas nos alertas ou identificadas durante as investigações.

  > **Observação:** ações de segurança no momento apenas dá suporte a permissões do aplicativo compatível.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter a ação de segurança](../api/securityaction-get.md) | [securityAction](securityaction.md) | Leia as propriedades e os relacionamentos do objeto securityAction. |
| [Criar ação de segurança](../api/securityactions-post.md) | [securityAction](securityaction.md) | Crie uma nova securityAction postando na coleção securityActions. |
| [Listar ações de segurança](../api/securityactions-list.md) | [coleção securityAction](securityaction.md) | Obter uma coleção de objetos securityAction. |
|[Cancelar ação de segurança](../api/securityaction-cancelsecurityaction.md)|Nenhum(a)|Cancelar uma operação de segurança.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|actionReason|String|Motivo para invocar essa ação.|
|appId|String|A ID do Aplicativo do aplicativo de chamada que enviou a ação (POST). A appId deve ser extraída do token de auth e não inserida manualmente pelo aplicativo de chamada.|
|azureTenantId|String|ID de locatário do Azure da entidade para determinar a qual locatário a entidade pertence (suporte a multilocatária). A azureTenantId deve ser extraída do token de auth e não inserida manualmente pelo aplicativo de chamada.|
|completedDateTime|DateTimeOffset|Timestamp quando a ação foi concluída. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|createdDateTime|DateTimeOffset|Timestamp quando a ação é criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|errorInfo|[resultInfo](resultinfo.md)| Informações de erro quando a ação falha.|
|id|String| Criado pelo sistema quando a ação é ingerida. Identificador GUID/exclusivo gerado. Somente leitura.|
|lastActionDateTime|DateTimeOffset| Timestamp quando esta ação foi atualizada pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|name|String| Nome da ação.|
|parameters|Coleção [keyValuePair](keyvaluepair.md)| Coleção de parâmetros (pares chave-valor) necessários para invocar a ação, por exemplo, URL ou fileHash para bloquear, etc.). **Required**|
|estados|[Coleção securityActionState](securityactionstate.md)|Coleção de securityActionState para manter o histórico de uma ação.|
|status|cadeia de caracteres| Status da ação. Os valores possíveis são: `NotStarted`, `Running`, `Completed`, `Failed`.|
|user|String| O nome principal do usuário do usuário que enviou (POST) a ação. O usuário deve ser extraído do token de auth e não inserido manualmente pelo aplicativo de chamada.|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|Tipo complexo contendo detalhes sobre o fornecedor, provedor e subprovedor de produtos/serviços de segurança (por exemplo, vendor=Microsoft; provider=Windows Defender ATP; sub-provider=AppLocker).|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityAction",
  "keyProperty": "id"
}-->

```json
{
  "actionReason": "String",
  "appId": "String",
  "azureTenantId": "String",
  "clientContext": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "errorInfo": {"@odata.type": "microsoft.graph.resultInfo"},
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "states": [{"@odata.type": "microsoft.graph.securityActionState"}],
  "status": "string",
  "user": "String",
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->