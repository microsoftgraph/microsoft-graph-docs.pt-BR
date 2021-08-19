---
title: Tipo de recurso expeditedWindowsQualityUpdateSettings
description: Um tipo complexo para armazenar as configurações de atualização de qualidade aceleradas, como data e dias de lançamento até a reinicialização forçada.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8537f7bf9736d5d6e2a7015d3d1f11af7f7be0710698e964465d41311543e3f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54193528"
---
# <a name="expeditedwindowsqualityupdatesettings-resource-type"></a>Tipo de recurso expeditedWindowsQualityUpdateSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um tipo complexo para armazenar as configurações de atualização de qualidade aceleradas, como data e dias de lançamento até a reinicialização forçada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|qualityUpdateRelease|Cadeia de caracteres|A data de lançamento para identificar uma atualização de qualidade.|
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




