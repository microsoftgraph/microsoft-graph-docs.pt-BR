---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4778e01076e2af1c18edb16a2587f65396cc6466
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977245"
---
# <a name="auditresource-resource-type"></a>Tipo de recurso auditResource

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma classe que contém as propriedades para o Recurso de auditoria.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição.|
|ModifiedProperties|Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)|Lista de propriedades modificadas.|
|tipo|Cadeia de caracteres|Tipo de recurso de auditoria.|
|resourceId|Cadeia de caracteres|ID do recurso de auditoria.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```



