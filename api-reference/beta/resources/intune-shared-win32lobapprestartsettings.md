---
title: Tipo de recurso win32LobAppRestartSettings
description: Contém propriedades que descrevem a coordenação de reinicialização após uma instalação do aplicativo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1db6681ca521224ec99abc36e7058a414e7e7b2c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59051108"
---
# <a name="win32lobapprestartsettings-resource-type"></a>Tipo de recurso win32LobAppRestartSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades que descrevem a coordenação de reinicialização após uma instalação do aplicativo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|gracePeriodInMinutes|Int32|O número de minutos para aguardar antes de reiniciar o dispositivo após a instalação de um aplicativo.|
|countdownDisplayBeforeRestartInMinutes|Int32|O número de minutos antes da hora de reinicialização para exibir a caixa de diálogo de contagem regressiva para reinicializações pendentes.|
|restartNotificationSnoozeDurationInMinutes|Int32|O número de minutos para esnocar a caixa de diálogo de notificação de reinicialização quando o botão de esnooze estiver selecionado.|

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



