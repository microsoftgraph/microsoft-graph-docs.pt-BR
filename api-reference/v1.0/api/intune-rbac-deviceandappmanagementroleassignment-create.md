---
title: Criar deviceAndAppManagementRoleAssignment
description: Cria um novo objeto deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1a0d573e2636868ee6a37e96297e096a80c3a2fa
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52743221"
---
# <a name="create-deviceandappmanagementroleassignment"></a>Criar deviceAndAppManagementRoleAssignment

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Cria um novo objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementRBAC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementRBAC.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto deviceAndAppManagementRoleAssignment.

A tabela a seguir mostra as propriedades que são necessárias ao criar deviceAndAppManagementRoleAssignment.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. É somente leitura e gerada automaticamente. Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|displayName|Cadeia de caracteres|O nome de exibição ou nome amigável da atribuição de função. Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|descrição|Cadeia de caracteres|Descrição da atribuição de função. Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|resourceScopes|Coleção de cadeias de caracteres|Lista de IDs de grupos de segurança de membros de escopo da função.  Estas são as IDs do Azure Active Directory. Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|members|Coleção de cadeias de caracteres|A lista de IDs de grupos de segurança de membros da função. Estas são as IDs do Azure Active Directory.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```




