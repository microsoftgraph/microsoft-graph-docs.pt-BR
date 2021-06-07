---
title: Tipo de recurso managedAppPolicyDeploymentSummary
description: O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2198c84468585cf4dcc9bed365df4b8016fa5ef5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752333"
---
# <a name="managedapppolicydeploymentsummary-resource-type"></a>Tipo de recurso managedAppPolicyDeploymentSummary

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter managedAppPolicyDeploymentSummary](../api/intune-mam-managedapppolicydeploymentsummary-get.md)|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|Ler propriedades e relações de objetos de [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).|
|[Atualizar managedAppPolicyDeploymentSummary](../api/intune-mam-managedapppolicydeploymentsummary-update.md)|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|Atualizar as propriedades de um objeto de [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Ainda não documentado|
|configurationDeployedUserCount|Int32|Ainda não documentado|
|lastRefreshTime|DateTimeOffset|Ainda não documentado|
|configurationDeploymentSummaryPerApp|Conjunto [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)|Ainda não documentado|
|id|Cadeia de caracteres|Chave da entidade.|
|versão|String|Versão da entidade.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "String",
  "configurationDeployedUserCount": 1024,
  "lastRefreshTime": "String (timestamp)",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "String"
      },
      "configurationAppliedUserCount": 1024
    }
  ],
  "id": "String (identifier)",
  "version": "String"
}
```




