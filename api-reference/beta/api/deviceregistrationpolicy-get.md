---
title: Obter deviceRegistrationPolicy
description: Leia as propriedades e as relações de um objeto deviceRegistrationPolicy.
author: spunukol
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b02e1c9d6a0de046771e4a437cb1762eea73c6db
ms.sourcegitcommit: 2f394a9f33f2fab3634d0f18882985ee211067d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2021
ms.locfileid: "60127894"
---
# <a name="get-deviceregistrationpolicy"></a>Obter deviceRegistrationPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto deviceRegistrationPolicy.](../resources/deviceregistrationpolicy.md) Representa restrições de cota deviceRegistrationPolicy, autenticação adicional e políticas de autorização para registrar identidades de dispositivos em sua organização.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)| Policy.ReadWrite.DeviceConfiguration|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|Sem suporte|

Ao chamar em nome de um usuário, o usuário precisa pertencer às seguintes funções [do Azure AD:](/azure/active-directory/roles/permissions-reference)
+ Administrador global
+ Administrador de dispositivos de nuvem
+ Leitor global

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
```http
GET /policies/deviceRegistrationPolicy
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "get_deviceregistrationpolicy"
}
-->
``` http
GET https://graph.microsoft.com/policies/deviceRegistrationPolicy
```


### <a name="response"></a>Resposta

A seguir está um exemplo de uma resposta que mostra as configurações padrão da política de registro do dispositivo.

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
