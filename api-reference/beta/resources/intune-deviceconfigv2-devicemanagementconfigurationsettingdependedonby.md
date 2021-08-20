---
title: Tipo de recurso deviceManagementConfigurationSettingDependedOnBy
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8a82dc6f1c690ba745d29c042b7eb428adaf1c8dfd3339dfbadff45fd66588e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227390"
---
# <a name="devicemanagementconfigurationsettingdependedonby-resource-type"></a>Tipo de recurso deviceManagementConfigurationSettingDependedOnBy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|dependedOnBy|Cadeia de caracteres|Identificador da configuração filho que depende da configuração atual|
|obrigatório|Boolean|Valor que determina se a configuração filho é necessária com base na seleção da configuração pai|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
  "dependedOnBy": "String",
  "required": true
}
```




