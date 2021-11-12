---
title: Tipo de recurso securityAction
description: Executar uma ação imediata proteger contra ameaças usando a entidade securityActionde Segurança do Microsoft Graph. Quando um analista de segurança descobre um indicador novo, como um arquivo mal-intencionado, URL, domínio ou endereço IP, a proteção pode ser habilitada instantaneamente em suas soluções de segurança da Microsoft. Usar uma ação específica do provedor, ver todas as ações executadas e cancelar uma ação, se necessário. Experimente as ações de segurança com o ATP do Windows Defender (em breve) para bloquear as atividades mal-intencionados seus pontos de extremidade do Windows usando as propriedades vistas nos alertas ou identificadas durante as investigações.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7b7acb9da276e76b5e3245ffc787a2491a36537d
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60928477"
---
# <a name="securityaction-resource-type"></a>Tipo de recurso securityAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Executar uma ação imediata proteger contra ameaças usando a entidade securityActionde Segurança do Microsoft Graph. Quando um analista de segurança descobre um indicador novo, como um arquivo mal-intencionado, URL, domínio ou endereço IP, a proteção pode ser habilitada instantaneamente em suas soluções de segurança da Microsoft. Usar uma ação específica do provedor, ver todas as ações executadas e cancelar uma ação, se necessário. Experimente as ações de segurança com o [ATP do Windows Defender](/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection)para bloquear as atividades mal-intencionados em seus pontos de extremidade do Windows usando as propriedades vistas nos alertas ou identificadas durante as investigações.

  > **Observação:** ações de segurança no momento apenas dá suporte a permissões do aplicativo compatível.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter ações de segurança](../api/securityaction-get.md) | [securityAction](securityaction.md) | Ler propriedades e relações do objeto securityAction. |
| [Criar ação de segurança](../api/securityactions-post.md) | [securityAction](securityaction.md) | Crie uma nova securityAction postando na coleção securityActions. |
| [Listar ações de segurança](../api/securityactions-list.md) | [Coleção securityAction](securityaction.md) | Obter uma coleção de objetos securityAction. |
|[Cancelar ações de segurança](../api/securityaction-cancelsecurityaction.md)|Nenhum|Cancele uma operação de segurança.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|actionReason|Cadeia de caracteres|Motivo para invocar essa ação.|
|appId|Cadeia de caracteres|A ID do Aplicativo do aplicativo de chamada que enviou (POST) a ação. O appId deve ser extraído do token de auth e não inserido manualmente pelo aplicativo de chamada.|
|azureTenantId|String|ID do locatário do Azure da entidade para determinar a qual locatário a entidade pertence (suporte a vários locatários). O azureTenantId deve ser extraído do token de auth e não inserido manualmente pelo aplicativo de chamada.|
|completedDateTime|DateTimeOffset|Timestamp quando a ação foi concluída. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|createdDateTime|DateTimeOffset|Timestamp quando a ação é criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|errorInfo|[resultInfo](resultinfo.md)| Informações de erro quando a ação falhar.|
|id|Cadeia de caracteres| Criado pelo sistema quando a ação é ingerida. GUID gerado/identificador exclusivo. Somente leitura.|
|lastActionDateTime|DateTimeOffset| Timestamp quando essa ação foi atualizada pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|nome|Cadeia de caracteres| Nome da ação.|
|parameters|Coleção [keyValuePair](keyvaluepair.md)| Coleção de parâmetros (pares de valores-chave) necessários para invocar a ação, por exemplo, URL ou fileHash para bloquear.). **Obrigatório**.|
|states|[Coleção securityActionState](securityactionstate.md)|Coleção de securityActionState para manter o histórico de uma ação.|
|status|cadeia de caracteres| Status da ação. Os valores possíveis são: `NotStarted`, `Running`, `Completed`, `Failed`.|
|usuário|Cadeia de caracteres| O nome principal do usuário do usuário que enviou (POST) a ação. O usuário deve ser extraído do token de auth e não inserido manualmente pelo aplicativo de chamada.|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|Tipo complexo que contém detalhes sobre o fornecedor, provedor e sub-provedor de produtos/serviços de segurança (por exemplo, vendor=Microsoft; provider=Windows Defender ATP; sub-provider=AppLocker).|

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
