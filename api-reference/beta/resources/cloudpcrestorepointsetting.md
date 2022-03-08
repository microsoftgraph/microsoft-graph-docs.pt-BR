---
title: Tipo de recurso cloudPcRestorePointSetting
description: Representa configurações específicas de restauração point-in-time.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7e49cebd6f3bcb9a6af0ac469608b4c54081a7d8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338089"
---
# <a name="cloudpcrestorepointsetting-resource-type"></a>Tipo de recurso cloudPcRestorePointSetting

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de uma restauração point-in-time de um computador cloud.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|frequencyInHours|Int32|O intervalo de tempo em horas para tirar instantâneos (pontos de restauração) de um computador cloud automaticamente. Os valores possíveis `4`são , `6``12`, e `24``16`. A frequência padrão é de 12 horas.|
|userRestoreEnabled|Booliano|Se `true`, o usuário tem a capacidade de usar instantâneos para restaurar os PCs da Nuvem. Se `false`, os usuários que não são administradores não podem usar instantâneos para restaurar o Cloud PC.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcRestorePointSetting"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcRestorePointSetting",
  "frequencyInHours": "Integer",
  "userRestoreEnabled": "Boolean"
}
```
