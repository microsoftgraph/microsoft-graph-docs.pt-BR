---
title: Tipo de recurso hybridAgentUpdaterConfiguration
description: Tipo de recurso hybridAgentUpdaterConfiguration.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 39b378397b18337c660e76b815a80c9db398f950
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128600"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a>Tipo de recurso hybridAgentUpdaterConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um administrador de locatários pode configurar para cada onPremisesPublishingProfile a janela de tempo durante a qual os agentes podem receber atualizações ou adiar atualizações para os agentes. O hybridAgentUpdaterConfiguration especificado para um onPremisesPublishingProfile é aplicável a todos os agentes dentro desse onPremisesPublishingProfile.

Por exemplo, para os agentes em onPremisesPublishingProfile do tipo "provisionamento", as etapas poderiam ser as abaixo.

1) O administrador de locatários pode configurar para não receber atualizações dos agentes de provisionamento nos próximos n dias.
2) O administrador de locatários pode configurar uma janela de atualização (hora de início e de término) durante a qual os agentes podem recriar atualizações.
3) O administrador de locatários pode habilitar allowUpdateConfigurationOverride, que substitui a configuração do atualizador para agentes de provisionamento e permite que eles recebam a próxima atualização disponível.

As informações de Data/Hora especificadas na configuração do atualizador serão convertidas para o zona de hora local relatada pelo agente durante a confirmação.

A atualização do agente seguirá a lista de prioridades abaixo

1) Se allowUpdateConfigurationOverride for definido como verdadeiro, a configuração do atualizador definida pelo locatário será ignorada e o agente receberá uma atualização quando a próxima versão do agente estiver disponível (prioridade 1).
2) Se a atualização de adiamento estiver definida, o agente não será atualizado até a data e a hora da atualização de adiamento (prioridade 2).
3) Se a janela de atualização estiver definida, o agente será atualizado somente durante essa janela de tempo em um dia de 24 horas (prioridade 3).
4) Se nenhuma configuração do atualizador válida for definida pelo locatário, o agente receberá uma atualização quando a próxima versão do agente estiver disponível

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|allowUpdateConfigurationOverride|Boolean|Indica se a configuração do atualizador será ignorada e o agente receberá uma atualização quando a próxima versão do agente estiver disponível.|
|deferUpdateDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|updateWindow|[updateWindow](updatewindow.md)||

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
  "baseType": null
}-->

```json
{
  "allowUpdateConfigurationOverride": true,
  "deferUpdateDateTime": "String (timestamp)",
  "updateWindow": {"@odata.type": "microsoft.graph.updateWindow"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hybridAgentUpdaterConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


