---
title: Tipo de recurso deviceManagementConfigurationReferredSettingInformation
description: Informações de configuração referidas sobre a configuração reutilizável
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2a38d8566084999a291f770267745fe81015c5b9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58795526"
---
# <a name="devicemanagementconfigurationreferredsettinginformation-resource-type"></a>Tipo de recurso deviceManagementConfigurationReferredSettingInformation

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações de configuração referidas sobre a configuração reutilizável

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingDefinitionId|Cadeia de caracteres|Definindo a id de definição que está sendo referenciada a uma configuração. Aplicável para a configuração reutilizável|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
  "settingDefinitionId": "String"
}
```



