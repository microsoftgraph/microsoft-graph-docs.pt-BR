---
title: Tipo de recurso deviceManagementSettingAppConstraint
description: A restrição que aplica a configuração contém apenas tipos de aplicativos vaild.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f17221fae4db9d2aa0638d3cefc8a983b030abc81ade6817d386e36a297ee8c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251299"
---
# <a name="devicemanagementsettingappconstraint-resource-type"></a>Tipo de recurso deviceManagementSettingAppConstraint

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A restrição que aplica a configuração contém apenas tipos de aplicativos vaild.


Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|supportedTypes|String collection|Tipos de aplicativo aceitáveis para permitir essa configuração|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingAppConstraint",
  "supportedTypes": [
    "String"
  ]
}
```




