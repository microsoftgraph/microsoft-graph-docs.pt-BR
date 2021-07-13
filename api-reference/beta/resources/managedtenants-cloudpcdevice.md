---
title: Tipo de recurso cloudPcDevice
description: Representa um dispositivo de computador na nuvem que pertence a um determinado locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 57eabb6720987a8a9bfca4c18e283057848b65cf
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401945"
---
# <a name="cloudpcdevice-resource-type"></a>Tipo de recurso cloudPcDevice

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um dispositivo de computador na nuvem que pertence a um determinado locatário gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar cloudPcDevices](../api/managedtenants-managedtenant-list-cloudpcdevices.md)|[coleção microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md)|Obter uma lista dos objetos [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) e suas propriedades.|
|[Obter cloudPcDevice](../api/managedtenants-cloudpcdevice-get.md)|[microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md)|Leia as propriedades e as relações de um [objeto cloudPcDevice.](../resources/managedtenants-cloudpcdevice.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|cloudPcStatus|Cadeia de caracteres|O status do computador de nuvem. Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`. Obrigatório. Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição do computador de nuvem. Obrigatório. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo do computador de nuvem. Obrigatório. Somente leitura.|
|lastRefreshedDateTime|DateTimeOffset|Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento de vários locatários. Obrigatório. Somente leitura.|
|managedDeviceId|Cadeia de caracteres|O identificador de dispositivo gerenciado para o computador de nuvem. Opcional. Somente leitura.|
|managedDeviceName|String|O nome de exibição do dispositivo gerenciado para o computador de nuvem. Opcional. Somente leitura.|
|provisioningPolicyId|Cadeia de caracteres|O identificador de política de provisionamento para o computador de nuvem. Obrigatório. Somente leitura.|
|servicePlanName|Cadeia de caracteres|O nome do plano de serviço para o computador na nuvem. Obrigatório. Somente leitura.|
|tenantDisplayName|Cadeia de caracteres|O nome de exibição do locatário gerenciado. Obrigatório. Somente leitura.|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md) Obrigatório. Somente leitura.|
|userPrincipalName|Cadeia de caracteres|O nome principal do usuário (UPN) do usuário atribuído ao computador de nuvem. Obrigatório. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.cloudPcDevice",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcDevice",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "userPrincipalName": "String",
  "servicePlanName": "String",
  "cloudPcStatus": "String",
  "provisioningPolicyId": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
