---
title: tipo de recurso SecurityAction
description: Execute ações imediatas para se defender contra ameaças usando a entidade Security SecurityAction do Microsoft Graph. Quando um analista de segurança descobre um novo indicador, como um arquivo mal-intencionado, URL, domínio ou endereço IP, a proteção pode ser ativada instantaneamente em suas soluções de segurança da Microsoft. Invocar uma ação para um provedor específico, ver todas as ações realizadas e cancelar uma ação se necessário. Tente as ações de segurança com o Windows Defender ATP (em breve) para bloquear atividades mal-intencionadas em seus pontos de extremidade do Windows usando Propriedades vistas em alertas ou identificadas durante investigações.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 405f12c2cf484651f8bcefc791c9dd24dae410bd
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366984"
---
# <a name="securityaction-resource-type"></a>tipo de recurso SecurityAction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Execute ações imediatas para se defender contra ameaças usando a entidade Security SecurityAction do Microsoft Graph. Quando um analista de segurança descobre um novo indicador, como um arquivo mal-intencionado, URL, domínio ou endereço IP, a proteção pode ser ativada instantaneamente em suas soluções de segurança da Microsoft. Invocar uma ação para um provedor específico, ver todas as ações realizadas e cancelar uma ação se necessário. Tente as ações de segurança com o [Windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) (em breve) para bloquear atividades mal-intencionadas em seus pontos de extremidade do Windows usando Propriedades vistas em alertas ou identificadas durante investigações.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter SecurityAction](../api/securityaction-get.md) | [SecurityAction](securityaction.md) | Leia as propriedades e as relações do objeto SecurityAction. |
| [Criar SecurityAction](../api/securityactions-post.md) | [SecurityAction](securityaction.md) | Crie um novo SecurityAction postando na coleção securityActions. |
| [Listar securityActions](../api/securityactions-list.md) | [](securityaction.md) coleção SecurityAction | Obtenha uma coleção de objetos SecurityAction. |
|[Cancelar SecurityAction](../api/securityaction-cancelsecurityaction.md)|Nenhum|Cancela uma operação de segurança.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|actionReason|String|Motivo para invocar esta ação.|
|appId|String|A ID de aplicativo do aplicativo de chamada que enviou (POST) a ação. A appId deve ser extraída do token de autenticação e não inserida manualmente pelo aplicativo de chamada.|
|azureTenantId|String|ID do locatário do Azure da entidade para determinar a qual locatário a entidade pertence (suporte a várias locação). O azureTenantId deve ser extraído do token de autenticação e não é inserido manualmente pelo aplicativo de chamada.|
|completedDateTime|DateTimeOffset|Carimbo de data/hora em que a ação foi concluída. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|createdDateTime|DateTimeOffset|Carimbo de data/hora em que a ação é criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|errorInfo|[resultInfo](resultinfo.md)| Informações de erro quando a ação falha.|
|id|String| Criado pelo sistema quando a ação é ingerida. GUID gerado/identificador exclusivo. Somente leitura.|
|lastActionDateTime|DateTimeOffset| Carimbo de data/hora da última atualização da ação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|name|String| Nome da ação.|
|parâmetros|Coleção [keyValuePair](keyvaluepair.md)| Coleção de parâmetros (pares chave-valor) necessário para invocar a ação, por exemplo, URL ou fileHash para bloquear, etc.). **Required**|
|determina|coleção [securityActionState](securityactionstate.md)|Coleção de securityActionState para manter o histórico de uma ação.|
|status|string| Status da ação. Os valores possíveis são: `NotStarted`, `Running`, `Completed`, `Failed`.|
|user|String| O nome principal de usuário do usuário conectado que enviou (POST) a ação. O usuário deve ser extraído do token de autenticação e não inserido manualmente pelo aplicativo de chamada.|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|Tipo complexo que contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subprovedor (por exemplo, fornecedor = Microsoft; Provider = Windows Defender ATP; subprovider = AppLocker).|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityAction",
  "baseType": "",
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