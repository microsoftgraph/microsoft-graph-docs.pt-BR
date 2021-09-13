---
title: Tipo de recurso deviceManagementTroubleshootingErrorResource
description: Objeto que representa um link para a solução de problemas de informações, o link pode ser para o Portal do Azure ou um documento da Microsoft.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 524f5615e165f32a1b67341d5066b56414404e7f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039004"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a>Tipo de recurso deviceManagementTroubleshootingErrorResource

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Objeto que representa um link para a solução de problemas de informações, o link pode ser para o Portal do Azure ou um documento da Microsoft.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|texto|String|Ainda não documentado|
|link|Cadeia de Caracteres|O link para o recurso Web. Pode conter qualquer um dos seguintes formadores: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}|

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




