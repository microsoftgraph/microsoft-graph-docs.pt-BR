---
title: Tipo de recurso deviceManagementTroubleshootingErrorResource
description: Objeto que representa um link para a solução de problemas de informações, o link pode ser para o Portal do Azure ou um documento da Microsoft.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1da7b75414aafcce5e221cbb5f6e0cfc0ea0209b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266790"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a>Tipo de recurso deviceManagementTroubleshootingErrorResource

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Objeto que representa um link para a solução de problemas de informações, o link pode ser para o Portal do Azure ou um documento da Microsoft.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|texto|String|Ainda não documentado|
|link|Cadeia de caracteres|O link para o recurso Web. Pode conter qualquer um dos seguintes formadores: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorResource",
  "text": "String",
  "link": "String"
}
```




