---
title: Tipo de recurso chromeOSDeviceProperty
description: Representa uma propriedade do dispositivo ChromeOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 42b4903965d90641955659277360c46428562ed4
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666755"
---
# <a name="chromeosdeviceproperty-resource-type"></a>Tipo de recurso chromeOSDeviceProperty

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa uma propriedade do dispositivo ChromeOS.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|String|Nome da propriedade|
|value|Cadeia de caracteres|Valor da propriedade|
|valueType|String|Tipo do valor|
|atualizável|Booleano|Se essa propriedade é atualizável|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chromeOSDeviceProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chromeOSDeviceProperty",
  "name": "String",
  "value": "String",
  "valueType": "String",
  "updatable": true
}
```




