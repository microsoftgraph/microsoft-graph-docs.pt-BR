---
title: Tipo de recurso deviceManagementConfigurationSettingValueTemplateReference
description: Definindo informações de referência do modelo de valor
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 85ba2f21b8de862952535cf952aac1712c201f29a138cc5d03cddd4233862d1d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54127009"
---
# <a name="devicemanagementconfigurationsettingvaluetemplatereference-resource-type"></a>Tipo de recurso deviceManagementConfigurationSettingValueTemplateReference

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definindo informações de referência do modelo de valor

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingValueTemplateId|Cadeia de caracteres|Definindo a id do modelo de valor|
|useTemplateDefault|Boolean|Indica se o valor de configuração da política deve ser atualizado para corresponder ao valor padrão da configuração do modelo|

## <a name="relationships"></a>Relações
Nenhum

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




