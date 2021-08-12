---
title: Tipo de recurso win32LobAppRestartSettings
description: Contém propriedades que descrevem a coordenação de reinicialização após uma instalação do aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3f786a52c2a572ccaa1ba1fd7bea9e0c1f6b2358f238144f638c94dc6c48efde
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54175249"
---
# <a name="win32lobapprestartsettings-resource-type"></a>Tipo de recurso win32LobAppRestartSettings

Namespace: microsoft.graph

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




