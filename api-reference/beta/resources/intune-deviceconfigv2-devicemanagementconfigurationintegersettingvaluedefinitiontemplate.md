---
title: Tipo de recurso deviceManagementConfigurationIntegerSettingValueDefinitionTemplate
description: Modelo de definição de valor de configuração de inteiro
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6aa5571402ccddf6cf5524e2e2486caffcc550c7
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820720"
---
# <a name="devicemanagementconfigurationintegersettingvaluedefinitiontemplate-resource-type"></a>Tipo de recurso deviceManagementConfigurationIntegerSettingValueDefinitionTemplate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modelo de definição de valor de configuração de inteiro

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|minValue|Int32|Valor mínimo de configuração de inteiro. Valores válidos -2147483648 para 2147483647|
|maxValue|Int32|Valor máximo de configuração de inteiro. Valores válidos -2147483648 para 2147483647|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate",
  "minValue": 1024,
  "maxValue": 1024
}
```



