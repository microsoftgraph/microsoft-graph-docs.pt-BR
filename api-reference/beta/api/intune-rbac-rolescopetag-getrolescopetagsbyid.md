---
title: Ação getRoleScopeTagsById
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eb1f92ca2e0d803eb4f2ab579d6109e22ec40563
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58801238"
---
# <a name="getrolescopetagsbyid-action"></a>Ação getRoleScopeTagsById

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.Read.All, DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags/getRoleScopeTagsById
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/getRoleScopeTagsById
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|roleScopeTagIds|String collection|Ainda não documentado|



## <a name="response"></a>Resposta
Se tiver êxito, essa ação retornará `200 OK` um código de resposta e uma coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/getRoleScopeTagsById

Content-type: application/json
Content-length: 65

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTag",
      "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
      "displayName": "Display Name value",
      "description": "Description value",
      "isBuiltIn": true
    }
  ]
}
```



