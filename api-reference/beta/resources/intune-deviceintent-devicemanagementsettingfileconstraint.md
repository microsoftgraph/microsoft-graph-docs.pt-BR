---
title: Tipo de recurso deviceManagementSettingFileConstraint
description: A restrição de imposição da extensão de arquivo é aceitável para uma determinada configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3cdca0f1cba17381809fa87bea1400020875c2c67c8abfa3dcf5bf4ca540f44b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54193682"
---
# <a name="devicemanagementsettingfileconstraint-resource-type"></a>Tipo de recurso deviceManagementSettingFileConstraint

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A restrição de imposição da extensão de arquivo é aceitável para uma determinada configuração


Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|supportedExtensions|String collection|Extensões de arquivo aceitáveis para carregar para essa configuração|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingFileConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingFileConstraint",
  "supportedExtensions": [
    "String"
  ]
}
```




