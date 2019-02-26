---
title: tipo de recurso windows10AssociatedApps
description: Definição de aplicativo associado ao Windows 10.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 95f0114bbd39e85c137da2a71b7640ba8051b6dc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146680"
---
# <a name="windows10associatedapps-resource-type"></a>tipo de recurso windows10AssociatedApps

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição de aplicativo associado ao Windows 10.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appType|[windows10AppType](../resources/intune-deviceconfig-windows10apptype.md)|Tipo de aplicativo. Os valores possíveis são: `desktop` e `universal`.|
|identificador|String|Identificação.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```




