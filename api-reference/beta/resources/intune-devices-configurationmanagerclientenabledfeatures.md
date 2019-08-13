---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d9407e1d035a5cd50db7b071f562acb4eb2d007b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371982"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>Tipo de recurso configurationManagerClientEnabledFeatures

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

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
|endpointProtection|Booliano|Se o Endpoint Protection é gerenciado pelo Intune|
|Officetreinamento|Booliano|Se o aplicativo do Office é gerenciado pelo Intune|

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



