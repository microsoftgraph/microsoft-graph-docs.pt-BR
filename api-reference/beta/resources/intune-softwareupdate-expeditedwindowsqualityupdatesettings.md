---
title: Tipo de recurso expeditedWindowsQualityUpdateSettings
description: Um tipo complexo para armazenar as configurações de atualização de qualidade aceleradas, como data e dias de lançamento até a reinicialização forçada.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 127a5ec4e1650cdd4e24787e24757b05732284d3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59029917"
---
# <a name="expeditedwindowsqualityupdatesettings-resource-type"></a>Tipo de recurso expeditedWindowsQualityUpdateSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um tipo complexo para armazenar as configurações de atualização de qualidade aceleradas, como data e dias de lançamento até a reinicialização forçada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|qualityUpdateRelease|Cadeia de Caracteres|A data de lançamento para identificar uma atualização de qualidade.|
|daysUntilForcedReboot|Int32|O número de dias após a instalação que a reinicialização forçada acontecerá.|

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



