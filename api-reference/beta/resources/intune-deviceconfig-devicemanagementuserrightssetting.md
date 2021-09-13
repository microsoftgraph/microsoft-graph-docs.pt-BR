---
title: Tipo de recurso deviceManagementUserRightsSetting
description: Representa uma configuração de direitos do usuário.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c6f4073fc471d4db16c9d41b77534975284b1bd7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054545"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a>Tipo de recurso deviceManagementUserRightsSetting

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa uma configuração de direitos do usuário.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|state|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Representando o estado atual dessa configuração de direitos de usuário. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|localUsersOrGroups|[Coleção deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)|Representando uma coleção de usuários locais ou grupos que serão definidos no dispositivo se o estado dessa configuração for Permitido. Esta coleção pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsSetting",
  "state": "String",
  "localUsersOrGroups": [
    {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
      "name": "String",
      "description": "String",
      "securityIdentifier": "String"
    }
  ]
}
```



