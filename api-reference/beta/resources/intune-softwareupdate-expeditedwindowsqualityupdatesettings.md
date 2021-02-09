---
title: Tipo de recurso expeditedWindowsQualityUpdateSettings
description: Um tipo complexo para armazenar as configurações de atualização de qualidade aceleradas, como data de lançamento e dias até a reinicialização forçada.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 700b86d15737c75cbf10679ea6e944726d667431
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160071"
---
# <a name="expeditedwindowsqualityupdatesettings-resource-type"></a>Tipo de recurso expeditedWindowsQualityUpdateSettings

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um tipo complexo para armazenar as configurações de atualização de qualidade aceleradas, como data de lançamento e dias até a reinicialização forçada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|qualityUpdateRelease|String|A data de lançamento para identificar uma atualização de qualidade.|
|daysUntilForcedReboot|Int32|O número de dias após a instalação que a reinicialização forçada ocorrerá.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.expeditedWindowsQualityUpdateSettings",
  "qualityUpdateRelease": "String",
  "daysUntilForcedReboot": 1024
}
```




