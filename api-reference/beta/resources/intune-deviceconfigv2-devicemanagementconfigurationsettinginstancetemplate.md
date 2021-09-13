---
title: Tipo de recurso deviceManagementConfigurationSettingInstanceTemplate
description: Modelo de instância de configuração
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 13da26610afbfcdc0c44d8724c661ab6ba4effb8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148407"
---
# <a name="devicemanagementconfigurationsettinginstancetemplate-resource-type"></a>Tipo de recurso deviceManagementConfigurationSettingInstanceTemplate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modelo de instância de configuração

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingInstanceTemplateId|Cadeia de Caracteres|Id do modelo de instância de configuração|
|settingDefinitionId|Cadeia de Caracteres|Definindo id de definição|
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



