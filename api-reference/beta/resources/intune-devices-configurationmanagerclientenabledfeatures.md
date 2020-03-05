---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2dfae041f1aab4c4ea74490d372350c5c0c2087b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528679"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>Tipo de recurso configurationManagerClientEnabledFeatures

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

recursos habilitados pelo cliente do Gerenciador de Configurações

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|inventory|Boolean|Se o estoque é gerenciado pelo Intune|
|modernApps|Boolean|Se o aplicativo moderno é gerenciado pelo Intune|
|resourceAccess|Boolean|Se o acesso ao recurso é gerenciado pelo Intune|
|deviceConfiguration|Boolean|Se a configuração do dispositivo é gerenciada pelo Intune|
|compliancePolicy|Boolean|Se a política de conformidade é gerenciada pelo Intune|
|windowsUpdateForBusiness|Booliano|Se o Windows Update para Empresas é gerenciado pelo Intune|
|endpointProtection|Boolean|Se o Endpoint Protection é gerenciado pelo Intune|
|Officetreinamento|Boolean|Se o aplicativo do Office é gerenciado pelo Intune|

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
  "windowsUpdateForBusiness": true,
  "endpointProtection": true,
  "officeApps": true
}
```



