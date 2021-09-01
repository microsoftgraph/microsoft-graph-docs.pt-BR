---
title: Tipo de recurso windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
description: Contém propriedades para o estado de implantação de uma política suplementar WindowsDefenderApplicationControl para um dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e7a7c52faf85a807027b3f73076680ed3d1609a9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58782886"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-resource-type"></a>Tipo de recurso windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o estado de implantação de uma política suplementar WindowsDefenderApplicationControl para um dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatuses](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-list.md)|[coleção windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Listar propriedades e relações dos [objetos windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|
|[Obter windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-get.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Leia propriedades e relações do [objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|
|[Criar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-create.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Crie um novo [objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|
|[Excluir windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-delete.md)|Nenhum(a)|Exclui um [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md).|
|[Atualizar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-update.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Atualize as propriedades de um [objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|deviceName|Cadeia de caracteres|Nome do dispositivo.|
|deviceId|Cadeia de caracteres|ID do dispositivo.|
|lastSyncDateTime|DateTimeOffset|Hora da última sincronização.|
|osVersion|String|Windows Versão do sistema operacional.|
|osDescription|Cadeia de caracteres|Windows Descrição da versão do sistema operacional.|
|deploymentStatus|[windowsDefenderApplicationControlSupplementalPolicyStatuses](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|O estado de implantação da política. Os valores possíveis são: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.|
|userName|Cadeia de caracteres|O nome do usuário deste dispositivo.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário.|
|policyVersion|Cadeia de caracteres|Versão acessível humana da política suplementar WindowsDefenderApplicationControl.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|política|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|O link de navegação para a política suplementar WindowsDefenderApplicationControl.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "osVersion": "String",
  "osDescription": "String",
  "deploymentStatus": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "policyVersion": "String"
}
```



