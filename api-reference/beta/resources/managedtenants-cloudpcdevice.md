---
title: Tipo de recurso cloudPcDevice
description: Representa um dispositivo de computador na nuvem que pertence a um determinado locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: f45893c100f335c34d700ba4eef07074469fa97c
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61862343"
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
|cloudPcStatus|String|O status do computador de nuvem. Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`. Obrigatório. Somente leitura.|
|displayName|String|O nome de exibição do computador de nuvem. Obrigatório. Somente leitura.|
|id|String|O identificador exclusivo do computador de nuvem. Obrigatório. Somente leitura.|
|lastRefreshedDateTime|DateTimeOffset|Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento de vários locatários. Obrigatório. Somente leitura.|
|managedDeviceId|String|O identificador de dispositivo gerenciado para o computador de nuvem. Opcional. Somente leitura.|
|managedDeviceName|String|O nome de exibição do dispositivo gerenciado para o computador de nuvem. Opcional. Somente leitura.|
|provisioningPolicyId|String|O identificador de política de provisionamento para o computador de nuvem. Obrigatório. Somente leitura.|
|servicePlanName|Cadeia de caracteres|O nome do plano de serviço para o computador na nuvem. Obrigatório. Somente leitura.|
|tenantDisplayName|String|O nome de exibição do locatário gerenciado. Obrigatório. Somente leitura.|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md) Obrigatório. Somente leitura.|
|userPrincipalName|String|O nome principal do usuário (UPN) do usuário atribuído ao computador de nuvem. Obrigatório. Somente leitura.|

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
