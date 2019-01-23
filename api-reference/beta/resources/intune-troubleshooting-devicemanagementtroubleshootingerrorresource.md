---
title: tipo de recurso de deviceManagementTroubleshootingErrorResource
description: Objeto que representa um link para obter informações, o link de solução de problemas poderia ser o Portal do Windows Azure ou um doc da Microsoft.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5653801fb3e4575e642c012721b667f51e791cc1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429250"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a>tipo de recurso de deviceManagementTroubleshootingErrorResource

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Objeto que representa um link para obter informações, o link de solução de problemas poderia ser o Portal do Windows Azure ou um doc da Microsoft.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|texto|String|Ainda não documentado|
|vínculo|String|O link para o recurso da web. Pode conter qualquer um dos formatadores a seguir: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}|

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




