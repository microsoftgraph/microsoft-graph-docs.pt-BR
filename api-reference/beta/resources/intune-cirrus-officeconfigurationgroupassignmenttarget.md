---
title: tipo de recurso de officeConfigurationGroupAssignmentTarget
description: Configuração de cliente do Office AAD destino de atribuição de grupo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b2fe6a668c1f490c167fe61496af14cf2654cebb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814767"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a>tipo de recurso de officeConfigurationGroupAssignmentTarget

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configuração de cliente do Office AAD destino de atribuição de grupo.

Herda de [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|groupId|Cadeia de caracteres|A identificação do grupo AAD pretendemos a configuração do dispositivo.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



