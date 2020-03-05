---
title: tipo de recurso SecurityAction
description: Executar uma ação imediata proteger contra ameaças usando a entidade securityActionde Segurança do Microsoft Graph. Quando um analista de segurança descobre um indicador novo, como um arquivo mal-intencionado, URL, domínio ou endereço IP, a proteção pode ser habilitada instantaneamente em suas soluções de segurança da Microsoft. Usar uma ação específica do provedor, ver todas as ações executadas e cancelar uma ação, se necessário. Experimente as ações de segurança com o ATP do Windows Defender (em breve) para bloquear as atividades mal-intencionados seus pontos de extremidade do Windows usando as propriedades vistas nos alertas ou identificadas durante as investigações.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 48c00d99ade3601e051d074272793d6aa0f2c66b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520826"
---
# <a name="securityaction-resource-type"></a>tipo de recurso SecurityAction

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Executar uma ação imediata proteger contra ameaças usando a entidade securityActionde Segurança do Microsoft Graph. Quando um analista de segurança descobre um indicador novo, como um arquivo mal-intencionado, URL, domínio ou endereço IP, a proteção pode ser habilitada instantaneamente em suas soluções de segurança da Microsoft. Usar uma ação específica do provedor, ver todas as ações executadas e cancelar uma ação, se necessário. Experimente as ações de segurança com o [ATP do Windows Defender](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection)para bloquear as atividades mal-intencionados em seus pontos de extremidade do Windows usando as propriedades vistas nos alertas ou identificadas durante as investigações.

  > **Observação:** ações de segurança no momento apenas dá suporte a permissões do aplicativo compatível.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter a ação de segurança](../api/securityaction-get.md) | [SecurityAction](securityaction.md) | Leia as propriedades e as relações do objeto SecurityAction. |
| [Criar ação de segurança](../api/securityactions-post.md) | [SecurityAction](securityaction.md) | Crie um novo SecurityAction postando na coleção securityActions. |
| [Listar ações de segurança](../api/securityactions-list.md) | coleção [SecurityAction](securityaction.md) | Obtenha uma coleção de objetos SecurityAction. |
|[Cancelar ação de segurança](../api/securityaction-cancelsecurityaction.md)|Nenhum|Cancela uma operação de segurança.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|actionReason|String|Motivo para invocar esta ação.|
|appId|String|A ID de aplicativo do aplicativo de chamada que enviou (POST) a ação. A appId deve ser extraída do token de autenticação e não inserida manualmente pelo aplicativo de chamada.|
|azureTenantId|String|ID do locatário do Azure da entidade para determinar a qual locatário a entidade pertence (suporte a várias locação). O azureTenantId deve ser extraído do token de autenticação e não é inserido manualmente pelo aplicativo de chamada.|
|completedDateTime|DateTimeOffset|Carimbo de data/hora em que a ação foi concluída. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|createdDateTime|DateTimeOffset|Carimbo de data/hora em que a ação é criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|errorInfo|[resultInfo](resultinfo.md)| Informações de erro quando a ação falha.|
|id|String| Criado pelo sistema quando a ação é ingerida. GUID gerado/identificador exclusivo. Somente leitura.|
|lastActionDateTime|DateTimeOffset| Carimbo de data/hora da última atualização da ação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|nome|String| Nome da ação.|
|parameters|Coleção [keyValuePair](keyvaluepair.md)| Coleção de parâmetros (pares chave-valor) necessário para invocar a ação, por exemplo, URL ou FileHash para bloquear, etc.). **Required**|
|determina|coleção [securityActionState](securityactionstate.md)|Coleção de securityActionState para manter o histórico de uma ação.|
|status|cadeia de caracteres| Status da ação. Os valores possíveis são: `NotStarted`, `Running`, `Completed`, `Failed`.|
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