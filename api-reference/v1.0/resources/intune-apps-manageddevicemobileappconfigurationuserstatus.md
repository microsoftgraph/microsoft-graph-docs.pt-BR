---
title: Tipo de recurso managedDeviceMobileAppConfigurationUserStatus
description: Contém propriedades, propriedades herdadas e ações para um status de configuração do aplicativo móvel de MDM para um usuário.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 806b0dd2351a355a32fa457522428138dd9e11fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531164"
---
# <a name="manageddevicemobileappconfigurationuserstatus-resource-type"></a>Tipo de recurso managedDeviceMobileAppConfigurationUserStatus

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades, propriedades herdadas e ações para um status de configuração do aplicativo móvel de MDM para um usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDeviceMobileAppConfigurationUserStatuses](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-list.md)|Conjunto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|Listar propriedades e relações de objetos de [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).|
|[Obter managedDeviceMobileAppConfigurationUserStatus](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-get.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).|
|[Criar managedDeviceMobileAppConfigurationUserStatus](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-create.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|Criar um novo objeto de [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).|
|[Excluir managedDeviceMobileAppConfigurationUserStatus](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-delete.md)|Nenhum|Excluir [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).|
|[Atualizar managedDeviceMobileAppConfigurationUserStatus](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-update.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|userDisplayName|Cadeia de caracteres|Nome de usuário de DevicePolicyStatus.|
|devicesCount|Int32|Contagem de dispositivos para esse usuário.|
|status|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Status de conformidade do relatório de políticas. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Data e hora da última modificação do relatório de políticas.|
|userPrincipalName|String|UserPrincipalName.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```




