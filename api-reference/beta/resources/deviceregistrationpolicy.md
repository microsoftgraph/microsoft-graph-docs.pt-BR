---
title: Tipo de recurso deviceRegistrationPolicy
description: Representa o escopo de política que controla restrições de cota, autenticação adicional e políticas de autorização para o Azure Active Directory locatário.
author: spunukol
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6b2fd1ac5d887aa324f4db898e3532c153c7a09c
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226747"
---
# <a name="deviceregistrationpolicy-resource-type"></a>Tipo de recurso deviceRegistrationPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o escopo de política que controla restrições de cota, autenticação adicional e políticas de autorização para registrar identidades de dispositivos em sua organização.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceRegistrationPolicy](../api/deviceregistrationpolicy-get.md)|[deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md)|Leia as propriedades de um [objeto deviceRegistrationPolicy.](../resources/deviceregistrationpolicy.md)|
|[Atualizar deviceRegistrationPolicy](../api/deviceregistrationpolicy-update.md)|[deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md)|Atualize as propriedades de um [objeto deviceRegistrationPolicy.](../resources/deviceregistrationpolicy.md)|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|azureADJoin|[azureAdJoinPolicy](../resources/azureadjoinpolicy.md)|Especifica a política de autorização para controlar o registro de novos dispositivos usando o **Azure AD Join** em sua organização. Obrigatório. Para obter mais informações, consulte [O que é uma identidade de dispositivo?](/azure/active-directory/devices/overview).|
|azureADRegistration|[azureADRegistrationPolicy](../resources/azureadregistrationpolicy.md)|Especifica a política de autorização para controlar o registro de novos dispositivos usando **o Azure AD registrado** em sua organização. Obrigatório. Para obter mais informações, consulte [O que é uma identidade de dispositivo?](/azure/active-directory/devices/overview).|
|description|String|A descrição da política de registro do dispositivo. Ele está sempre definido como `Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks` . Somente leitura.|
|displayName|String|O nome da política de registro do dispositivo. Ele está sempre definido como `Device Registration Policy` . Somente leitura.|
|id|String| O identificador da política de registro do dispositivo. Ele está sempre definido como `deviceRegistrationPolicy` . Apenas leitura.|
|multiFactorAuthConfiguration|multiFactorAuthConfiguration|Especifica a política de autenticação para um usuário concluir o registro usando o **Azure AD Join** ou **o Azure AD registrado** em sua organização. Os valores possíveis são: `0` (significado `notRequired` ), `1` (significado `required` ) e `2` (significado `unknownFutureValue` ). O valor padrão é `0`. |
|userDeviceQuota|Int32|Especifica o número máximo de dispositivos que um usuário pode ter em sua organização antes de bloquear novos registros de dispositivo. O valor padrão é definido como 50. Se essa propriedade não for especificada durante a operação de atualização de política, ela será redefinida automaticamente para indicar que os usuários não têm permissão para `0` ingressar em nenhum dispositivo. |


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
