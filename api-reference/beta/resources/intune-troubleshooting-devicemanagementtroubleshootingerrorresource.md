---
title: tipo de recurso deviceManagementTroubleshootingErrorResource
description: Objeto representando um link para informações de solução de problemas, o link pode ser para o portal do Azure ou um documento Microsoft.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 25d97a6d085b9f1b7e0b1ab73361be3ac7ae74d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155556"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a>tipo de recurso deviceManagementTroubleshootingErrorResource

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Objeto representando um link para informações de solução de problemas, o link pode ser para o portal do Azure ou um documento Microsoft.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|texto|String|Ainda não documentado|
|vínculo|String|O link para o recurso da Web. Pode conter qualquer um dos seguintes formatadores: {{UPN}}, {{DeviceGUID}}, {{userGUID}}|

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




