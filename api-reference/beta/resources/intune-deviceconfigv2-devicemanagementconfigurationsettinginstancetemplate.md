---
title: Tipo de recurso deviceManagementConfigurationSettingInstanceTemplate
description: Modelo de instância de configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4ebc516dc521c022a5b5a5e9eeb460dec3e4497
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58782109"
---
# <a name="devicemanagementconfigurationsettinginstancetemplate-resource-type"></a>Tipo de recurso deviceManagementConfigurationSettingInstanceTemplate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modelo de instância de configuração

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingInstanceTemplateId|Cadeia de caracteres|Id do modelo de instância de configuração|
|settingDefinitionId|Cadeia de caracteres|Definindo id de definição|
|isRequired|Booliano|Indica se uma política deve especificar essa configuração.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true
}
```



