---
title: tipo de recurso hybridAgentUpdaterConfiguration
description: tipo de recurso hybridAgentUpdaterConfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c10173d099ac7c2ad9714b0240f306e783fdd6da
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496807"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a>tipo de recurso hybridAgentUpdaterConfiguration

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um administrador de locatários pode configurar para cada onPremisesPublishingProfile a janela de tempo durante a qual os agentes podem receber atualizações ou adiar atualizações para os agentes. O hybridAgentUpdaterConfiguration especificado para um onPremisesPublishingProfile é aplicável a todos os agentes dentro desse onPremisesPublishingProfile.

Por exemplo, para os agentes no onPremisesPublishingProfile do tipo "Provisioning", as etapas podem ser as seguintes:

1) O administrador de locatários pode configurar o para não receber nenhuma atualização para os agentes de provisionamento nos próximos n dias.
2) O administrador de locatários pode configurar uma janela de atualização (hora de início e de término) durante a qual os agentes podem recive atualizações.
3) O administrador de locatários pode habilitar o allowUpdateConfigurationOverride que substitui o configutration atualizador de agentes de provisionamento e alows que eles recebam a próxima atualização disponível.

As informações de data/hora especificadas na configuração do atualizador serão convertidas no fuso horário local relatado pelo agente durante a evaluvation.

A atualização do agente seguirá a lista de prioridades abaixo

1) Se allowUpdateConfigurationOverride for definido como true, a configuração do atualizador definida pelo locatário será ignorada e o agente receberá uma atualização quando a próxima versão do agente estiver disponível (prioridade 1).
2) Se a atualização de adiamento estiver definida, o agente não será atualizado até a data de término da atualização (prioridade 2).
3) Se a janela de atualização for definida, o agente só será atualizado durante essa janela de tempo em um dia de 24 horas (prioridade 3).
4) Se nenhuma configuração válida do Updater for definida pelo locatário, o agente receberá uma atualização quando a próxima versão do agente estiver disponível

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
