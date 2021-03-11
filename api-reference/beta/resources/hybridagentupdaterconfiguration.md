---
title: Tipo de recurso hybridAgentUpdaterConfiguration
description: Tipo de recurso hybridAgentUpdaterConfiguration.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c81d48053e7fb26eaee678da4e4b33708717e3c1
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722395"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a>Tipo de recurso hybridAgentUpdaterConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um administrador de locatário pode configurar para cada onPremisesPublishingProfile a janela de tempo durante a qual os agentes podem receber atualizações ou adiar atualizações para os agentes. O hybridAgentUpdaterConfiguration especificado para um onPremisesPublishingProfile é aplicável a todos os agentes dentro desse onPremisesPublishingProfile.

Por exemplo, para os agentes em onPremisesPublishingProfile do tipo "provisionamento" as etapas podem ser as seguintes.

1) O administrador de locatários pode configurar para não receber atualizações para os agentes de Provisionamento para os próximos n dias.
2) O administrador de locatários pode configurar uma janela de atualização(início e hora de término) durante a qual os agentes podem realinhe as atualizações.
3) O administrador de locatários pode habilitar allowUpdateConfigurationOverride que substitui a configutração do atualizador para agentes de Provisionamento e permite que eles recebam a próxima atualização disponível.

As informações DateTime/Time especificadas na configuração do atualizador serão convertidas no zona de tempo local relatada pelo agente durante a evaluvação.

A atualização do agente seguirá a lista de prioridade abaixo

1) Se allowUpdateConfigurationOverride for definido como true, a configuração do updater definida pelo locatário será ignorada e o agente receberá uma atualização quando a próxima versão do agente estiver disponível (prioridade 1).
2) Se a atualização de adiamento estiver definida, o agente não será atualizado até a hora da atualização de adiamento (prioridade 2).
3) Se a janela de atualização estiver definida, o agente será atualizado somente durante essa janela de tempo em um dia de 24 horas (prioridade 3).
4) Se nenhuma configuração do atualizador válida for definida pelo locatário, o agente receberá uma atualização quando a próxima versão do agente estiver disponível

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|allowUpdateConfigurationOverride|Booliano|Indica se a configuração do atualizador será ignorada e o agente receberá uma atualização quando a próxima versão do agente estiver disponível.|
|deferUpdateDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
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


