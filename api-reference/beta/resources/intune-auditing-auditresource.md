---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: tfitzmac
ms.openlocfilehash: c60c76f899fabfbced271e6ec38043337b8b3851
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339862"
---
# <a name="auditresource-resource-type"></a>Tipo de recurso auditResource

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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





