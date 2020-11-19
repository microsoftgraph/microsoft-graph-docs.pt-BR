---
title: Acessar deviceAndAppManagementRoleDefinition
description: Leia as propriedades e as relações do objeto deviceAndAppManagementRoleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 30c4a5b6bb6efe385962933c544423c77ad2c478
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49210792"
---
# <a name="get-deviceandappmanagementroledefinition"></a><span data-ttu-id="608cf-103">Acessar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="608cf-103">Get deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="608cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="608cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="608cf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="608cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="608cf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="608cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="608cf-107">Leia as propriedades e as relações do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="608cf-107">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="608cf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="608cf-108">Prerequisites</span></span>
<span data-ttu-id="608cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="608cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="608cf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="608cf-111">Permission type</span></span>|<span data-ttu-id="608cf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="608cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="608cf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="608cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="608cf-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="608cf-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="608cf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="608cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="608cf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="608cf-116">Not supported.</span></span>|
|<span data-ttu-id="608cf-117">Application</span><span class="sxs-lookup"><span data-stu-id="608cf-117">Application</span></span>|<span data-ttu-id="608cf-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="608cf-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="608cf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="608cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="608cf-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="608cf-120">Optional query parameters</span></span>
<span data-ttu-id="608cf-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="608cf-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="608cf-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="608cf-122">Request headers</span></span>
|<span data-ttu-id="608cf-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="608cf-123">Header</span></span>|<span data-ttu-id="608cf-124">Valor</span><span class="sxs-lookup"><span data-stu-id="608cf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="608cf-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="608cf-125">Authorization</span></span>|<span data-ttu-id="608cf-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="608cf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="608cf-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="608cf-127">Accept</span></span>|<span data-ttu-id="608cf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="608cf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="608cf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="608cf-129">Request body</span></span>
<span data-ttu-id="608cf-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="608cf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="608cf-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="608cf-131">Response</span></span>
<span data-ttu-id="608cf-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="608cf-132">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="608cf-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="608cf-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="608cf-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="608cf-134">Request</span></span>
<span data-ttu-id="608cf-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="608cf-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="608cf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="608cf-136">Response</span></span>
<span data-ttu-id="608cf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="608cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1391

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
    "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
    "displayName": "Display Name value",
    "description": "Description value",
    "permissions": [
      {
        "@odata.type": "microsoft.graph.rolePermission",
        "actions": [
          "Actions value"
        ],
        "resourceActions": [
          {
            "@odata.type": "microsoft.graph.resourceAction",
            "allowedResourceActions": [
              "Allowed Resource Actions value"
            ],
            "notAllowedResourceActions": [
              "Not Allowed Resource Actions value"
            ]
          }
        ]
      }
    ],
    "rolePermissions": [
      {
        "@odata.type": "microsoft.graph.rolePermission",
        "actions": [
          "Actions value"
        ],
        "resourceActions": [
          {
            "@odata.type": "microsoft.graph.resourceAction",
            "allowedResourceActions": [
              "Allowed Resource Actions value"
            ],
            "notAllowedResourceActions": [
              "Not Allowed Resource Actions value"
            ]
          }
        ]
      }
    ],
    "isBuiltInRoleDefinition": true,
    "isBuiltIn": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




