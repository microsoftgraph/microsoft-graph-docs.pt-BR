---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 520b21445d4c5a61755ddc78c65b9999a7e45ff0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027493"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>Tipo de recurso configurationManagerClientEnabledFeatures

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

recursos habilitados pelo cliente do Gerenciador de Configurações

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|inventory|Booliano|Se o estoque é gerenciado pelo Intune|
|modernApps|Booliano|Se o aplicativo moderno é gerenciado pelo Intune|
|resourceAccess|Booliano|Se o acesso ao recurso é gerenciado pelo Intune|
|deviceConfiguration|Booliano|Se a configuração do dispositivo é gerenciada pelo Intune|
|compliancePolicy|Booliano|Se a política de conformidade é gerenciada pelo Intune|
|windowsUpdateForBusiness|Booliano|Se o Windows Update para Empresas é gerenciado pelo Intune|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```



