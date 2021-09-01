---
title: Tipo de recurso deviceManagementConfigurationDependentOn
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6a19f2b7ffe20954bf34cb01ffb0889c0294f56d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58784496"
---
# <a name="devicemanagementconfigurationdependenton-resource-type"></a>Tipo de recurso deviceManagementConfigurationDependentOn

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|dependentOn|Cadeia de caracteres|Identificador da opção de configuração pai/pai dependente|
|parentSettingId|Cadeia de caracteres|Identificador da id de configuração pai/configuração pai dependente de|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationDependentOn",
  "dependentOn": "String",
  "parentSettingId": "String"
}
```



