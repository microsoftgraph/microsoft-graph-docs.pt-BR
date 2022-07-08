---
title: Tipo de recurso deviceRegistrationPolicy
description: Representa o escopo da política que controla restrições de cota, autenticação adicional e políticas de autorização para o locatário do Azure Active Directory.
author: myra-ramdenbourg
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f810529cffc5c5c5c5a19d3fa2644aba5874d53e
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690074"
---
# <a name="deviceregistrationpolicy-resource-type"></a>Tipo de recurso deviceRegistrationPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o escopo da política que controla as restrições de cota, a autenticação adicional e as políticas de autorização para registrar identidades de dispositivo em sua organização.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceRegistrationPolicy](../api/deviceregistrationpolicy-get.md)|[deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md)|Leia as propriedades de um [objeto deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md) .|
|[Atualizar deviceRegistrationPolicy](../api/deviceregistrationpolicy-update.md)|[deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md)|Atualize as propriedades de [um objeto deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md) .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|azureADJoin|[azureAdJoinPolicy](../resources/azureadjoinpolicy.md)|Especifica a política de autorização para controlar o registro de novos dispositivos **Azure AD ingressar** em sua organização. Obrigatório. Para obter mais informações, consulte [O que é uma identidade do dispositivo?](/azure/active-directory/devices/overview).|
|azureADRegistration|[azureADRegistrationPolicy](../resources/azureadregistrationpolicy.md)|Especifica a política de autorização para controlar o registro de novos dispositivos **usando Azure AD registrados** em sua organização. Obrigatório. Para obter mais informações, consulte [O que é uma identidade do dispositivo?](/azure/active-directory/devices/overview).|
|descrição|Cadeia de caracteres|A descrição da política de registro do dispositivo. Ele é sempre definido como `Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks`. Somente leitura.|
|displayName|Cadeia de caracteres|O nome da política de registro do dispositivo. Ele é sempre definido como `Device Registration Policy`. Somente leitura.|
|id|Cadeia de caracteres| O identificador da política de registro do dispositivo. Ele é sempre definido como `deviceRegistrationPolicy`. Somente leitura.|
|multiFactorAuthConfiguration|multiFactorAuthConfiguration|Especifica a política de autenticação para que um usuário conclua o registro usando **Azure AD ingressar** ou Azure AD **registrado** em sua organização. Os valores possíveis são: `0` (significado `notRequired`), `1` (significado `required`) e `2` (significado `unknownFutureValue`). O valor padrão é `0`. |
|userDeviceQuota|Int32|Especifica o número máximo de dispositivos que um usuário pode ter em sua organização antes de bloquear novos registros de dispositivo. O valor padrão é definido como 50. Se essa propriedade não for especificada durante a operação de atualização de política, `0` ela será redefinida automaticamente para indicar que os usuários não têm permissão para ingressar em nenhum dispositivo. |


## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceRegistrationPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceRegistrationPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "userDeviceQuota": "Integer",
  "multiFactorAuthConfiguration": "String",
  "azureADRegistration": {
    "@odata.type": "microsoft.graph.azureADRegistrationPolicy"
  },
  "azureADJoin": {
    "@odata.type": "microsoft.graph.azureAdJoinPolicy"
  }
}
```
