---
title: Acessar roleDefinition
description: Leia as propriedades e as relações do objeto roleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: af6900bd995e8db8720f216b59dd077a872158b4
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37189323"
---
# <a name="get-roledefinition"></a><span data-ttu-id="57f15-103">Acessar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="57f15-103">Get roleDefinition</span></span>

> <span data-ttu-id="57f15-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57f15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57f15-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57f15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57f15-106">Leia as propriedades e as relações do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="57f15-106">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57f15-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57f15-107">Prerequisites</span></span>
<span data-ttu-id="57f15-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57f15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57f15-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57f15-110">Permission type</span></span>|<span data-ttu-id="57f15-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57f15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57f15-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57f15-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57f15-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="57f15-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="57f15-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57f15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57f15-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57f15-115">Not supported.</span></span>|
|<span data-ttu-id="57f15-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57f15-116">Application</span></span>|<span data-ttu-id="57f15-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="57f15-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57f15-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57f15-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57f15-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="57f15-119">Optional query parameters</span></span>
<span data-ttu-id="57f15-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="57f15-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57f15-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57f15-121">Request headers</span></span>
|<span data-ttu-id="57f15-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57f15-122">Header</span></span>|<span data-ttu-id="57f15-123">Valor</span><span class="sxs-lookup"><span data-stu-id="57f15-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57f15-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="57f15-124">Authorization</span></span>|<span data-ttu-id="57f15-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57f15-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57f15-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57f15-126">Accept</span></span>|<span data-ttu-id="57f15-127">application/json</span><span class="sxs-lookup"><span data-stu-id="57f15-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57f15-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57f15-128">Request body</span></span>
<span data-ttu-id="57f15-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57f15-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57f15-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="57f15-130">Response</span></span>
<span data-ttu-id="57f15-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57f15-131">If successful, this method returns a `200 OK` response code and [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57f15-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57f15-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="57f15-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57f15-133">Request</span></span>
<span data-ttu-id="57f15-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57f15-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="57f15-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="57f15-135">Response</span></span>
<span data-ttu-id="57f15-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57f15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1369

{
  "value": {
    "@odata.type": "#microsoft.graph.roleDefinition",
    "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
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




