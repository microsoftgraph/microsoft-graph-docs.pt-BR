---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f22ace5fa4c381584325ffc8434f0e09faaaaeb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156011"
---
# <a name="auditresource-resource-type"></a>Tipo de recurso auditResource

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades para o Recurso de auditoria.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome de exibição.|
|ModifiedProperties|Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)|Lista de propriedades modificadas.|
|tipo|String|Tipo de recurso de auditoria.|
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




