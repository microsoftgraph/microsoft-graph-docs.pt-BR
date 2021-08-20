---
title: Tipo de recurso deviceManagementSettingDependency
description: Informações de dependência para uma configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d5f29fecdde1b3a7a62ed72fcd96aceeb2a10385028106be288c7d8bcaff2254
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54173034"
---
# <a name="devicemanagementsettingdependency-resource-type"></a>Tipo de recurso deviceManagementSettingDependency

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações de dependência para uma configuração

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|definitionId|Cadeia de caracteres|A ID de definição de configuração da configuração dependia|
|restrições|[Coleção deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)|Coleção de restrições para o valor de configuração de dependência|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDependency",
  "definitionId": "String",
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "String"
      ]
    }
  ]
}
```




