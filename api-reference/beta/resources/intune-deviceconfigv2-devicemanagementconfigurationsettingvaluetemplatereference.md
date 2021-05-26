---
title: Tipo de recurso deviceManagementConfigurationSettingValueTemplateReference
description: Definindo informações de referência do modelo de valor
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fa4ecc07044d90bfc869467de8e8249f7581e228
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666769"
---
# <a name="devicemanagementconfigurationsettingvaluetemplatereference-resource-type"></a>Tipo de recurso deviceManagementConfigurationSettingValueTemplateReference

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definindo informações de referência do modelo de valor

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingValueTemplateId|String|Definindo a id do modelo de valor|
|useTemplateDefault|Booleano|Indica se o valor de configuração da política deve ser atualizado para corresponder ao valor padrão da configuração do modelo|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
  "settingValueTemplateId": "String",
  "useTemplateDefault": true
}
```




