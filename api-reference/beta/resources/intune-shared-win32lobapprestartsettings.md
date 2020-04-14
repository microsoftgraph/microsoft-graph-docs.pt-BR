---
title: tipo de recurso win32LobAppRestartSettings
description: Contém propriedades que descrevem a coordenação de reinicialização após uma instalação de aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e962c9e03a587f0393ddec1fe273be15c6547b22
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471994"
---
# <a name="win32lobapprestartsettings-resource-type"></a>tipo de recurso win32LobAppRestartSettings

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades que descrevem a coordenação de reinicialização após uma instalação de aplicativo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|gracePeriodInMinutes|Int32|O número de minutos de espera antes de reiniciar o dispositivo após uma instalação de aplicativo.|
|countdownDisplayBeforeRestartInMinutes|Int32|O número de minutos antes do tempo de reinicialização para exibir a caixa de diálogo de contagem regressiva de reinicializações pendentes.|
|restartNotificationSnoozeDurationInMinutes|Int32|O número de minutos para adiar a caixa de diálogo de notificação de reinicialização quando o botão adiar estiver selecionado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRestartSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRestartSettings",
  "gracePeriodInMinutes": 1024,
  "countdownDisplayBeforeRestartInMinutes": 1024,
  "restartNotificationSnoozeDurationInMinutes": 1024
}
```



