---
title: Atualizar deviceRegistrationPolicy
description: Atualize as propriedades de um objeto deviceRegistrationPolicy.
author: spunukol
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e55beac9f1ada8a3a6d2fe9d2ae8a81eff6e3085
ms.sourcegitcommit: 2f394a9f33f2fab3634d0f18882985ee211067d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2021
ms.locfileid: "60127895"
---
# <a name="update-deviceregistrationpolicy"></a>Atualizar deviceRegistrationPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto deviceRegistrationPolicy.](../resources/deviceregistrationpolicy.md) Representa restrições de cota deviceRegistrationPolicy, autenticação adicional e políticas de autorização para registrar identidades de dispositivos em sua organização.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Policy.ReadWrite.DeviceConfiguration|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|Sem suporte|

Ao chamar em nome de um usuário, o usuário precisa pertencer às seguintes funções [do Azure AD:](/azure/active-directory/roles/permissions-reference)
+ Administrador global
+ Administrador de dispositivos de nuvem

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
```http
PUT /policies/deviceRegistrationPolicy
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça *apenas* os valores das propriedades que devem ser atualizadas. As propriedades existentes que não estão incluídas no corpo da solicitação manterão seus valores anteriores ou serão recalculadas com base nas alterações em outros valores de propriedade.

A tabela a seguir especifica as propriedades que podem ser atualizadas.


|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userDeviceQuota|Int32|Especifica o número máximo de dispositivos que um usuário pode ter em sua organização antes de bloquear novos registros de dispositivo. |
|multiFactorAuthConfiguration|multiFactorAuthConfiguration|Especifica a política de autenticação para um usuário concluir o registro usando o Azure AD Join ou o Azure AD registrado em sua organização. Os valores possíveis são: `notRequired` ou `required`. |
|azureADRegistration|[azureADRegistrationPolicy](../resources/azureadregistrationpolicy.md)|Especifica a política de autorização para controlar o registro de novos dispositivos usando o registro do Azure AD em sua organização. Obrigatório. Para obter mais informações, consulte [O que é uma identidade de dispositivo?](/azure/active-directory/devices/overview). Se o Intune estiver habilitado, essa propriedade não poderá ser modificada.|
|azureADJoin|[azureAdJoinPolicy](../resources/azureadjoinpolicy.md)|Especifica a política de autorização para controlar o registro de novos dispositivos usando o Azure AD Join em sua organização. Obrigatório. Para obter mais informações, consulte [O que é uma identidade de dispositivo?](/azure/active-directory/devices/overview).|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "update_deviceregistrationpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/beta/deviceRegistrationPolicy
Content-Type: application/json

{
    "id": "deviceRegistrationPolicy",
    "displayName": "Device Registration Policy",
    "description": "Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks",
    "userDeviceQuota": 50,
    "multiFactorAuthConfiguration": "0",
    "azureADRegistration": {
        "appliesTo": "1",
        "isAdminConfigurable": false,
        "allowedUsers": [],
        "allowedGroups": []
    },
    "azureADJoin": {
        "appliesTo": "1",
        "isAdminConfigurable": true,
        "allowedUsers": [],
        "allowedGroups": []
    }
}
```

### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceRegistrationPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#deviceRegistrationPolicy",
    "id": "deviceRegistrationPolicy",
    "displayName": "Device Registration Policy",
    "description": "Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks",
    "userDeviceQuota": 50,
    "multiFactorAuthConfiguration": "0",
    "azureADRegistration": {
        "appliesTo": "1",
        "isAdminConfigurable": false,
        "allowedUsers": [],
        "allowedGroups": []
    },
    "azureADJoin": {
        "appliesTo": "1",
        "isAdminConfigurable": true,
        "allowedUsers": [],
        "allowedGroups": []
    }
}
```
