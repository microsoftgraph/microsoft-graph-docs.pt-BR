---
title: Tipo de recurso windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary
description: Contém propriedades para o resumo de implantação de uma política suplementar windowsDefenderApplicationControl.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 572788f0da665bfe717769b68fb3a06bfdb9b5b1db89c28dc192c7502acad2bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54181059"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-resource-type"></a>Tipo de recurso windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o resumo de implantação de uma política suplementar windowsDefenderApplicationControl.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-get.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|Leia propriedades e relações do [objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|
|[Atualizar windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-update.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|Atualize as propriedades de um [objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|deployedDeviceCount|Int32|Número de dispositivos que implantaram com êxito esta política suplementar WindowsDefenderApplicationControl.|
|failedDeviceCount|Int32|Número de dispositivos que falharam na implantação dessa política complementar windowsDefenderApplicationControl.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary",
  "id": "String (identifier)",
  "deployedDeviceCount": 1024,
  "failedDeviceCount": 1024
}
```




