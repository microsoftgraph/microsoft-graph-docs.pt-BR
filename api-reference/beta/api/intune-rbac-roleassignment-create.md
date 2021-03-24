---
title: Criar roleAssignment
description: Criar um novo objeto roleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c5b78b1b6d0dcfce3dfbba1fcb88c2d1c5159771
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148348"
---
# <a name="create-roleassignment"></a>Criar roleAssignment

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementRBAC.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementRBAC.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto roleAssignment.

A tabela a seguir mostra as propriedades que são necessárias ao criar roleAssignment.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. É somente leitura e gerada automaticamente.|
|displayName|Cadeia de caracteres|O nome de exibição ou nome amigável da atribuição de função.|
|descrição|Cadeia de caracteres|Descrição da atribuição de função.|
|scopeMembers|Coleção de cadeias de caracteres|Lista de IDs de grupos de segurança de membros de escopo da função.  Estas são as IDs do Azure Active Directory.|
|scopeType|[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)|Especifica o tipo de escopo de uma atribuição de função. O tipo padrão 'ResourceScope' permite a atribuição de ResourceScopes. Para 'AllDevices', 'AllLicensedUsers' e 'AllDevicesAndLicensedUsers', a propriedade ResourceScopes deve ser deixada vazia. Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.|
|resourceScopes|Coleção de cadeias de caracteres|Lista de IDs de grupos de segurança de membros de escopo da função.  Estas são as IDs do Azure Active Directory.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
Content-type: application/json
Content-length: 277

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 326

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```




