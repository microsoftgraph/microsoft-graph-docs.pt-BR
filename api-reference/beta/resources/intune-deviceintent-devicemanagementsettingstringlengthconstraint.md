---
title: Tipo de recurso deviceManagementSettingStringLengthConstraint
description: Restrição que aplica um determinado intervalo de comprimento de cadeia de caracteres
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4348ac61cd132e3ee361dd3ecc374d56d5bc177ca25521ab485b61718d00c439
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54172992"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a>Tipo de recurso deviceManagementSettingStringLengthConstraint

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Restrição que aplica um determinado intervalo de comprimento de cadeia de caracteres


Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|minimumLength|Int32|O comprimento mínimo permitido da cadeia de caracteres|
|maximumLength|Int32|O comprimento máximo permitido da cadeia de caracteres|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingStringLengthConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingStringLengthConstraint",
  "minimumLength": 1024,
  "maximumLength": 1024
}
```




