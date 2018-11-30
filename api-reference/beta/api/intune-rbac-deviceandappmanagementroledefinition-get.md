---
title: Acessar deviceAndAppManagementRoleDefinition
description: Leia as propriedades e as relações do objeto deviceAndAppManagementRoleDefinition.
ms.openlocfilehash: 0aef6b4eb7d2bc0c072bfa37cc1d0fa32801e670
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27032898"
---
# <a name="get-deviceandappmanagementroledefinition"></a><span data-ttu-id="0ec72-103">Acessar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0ec72-103">Get deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="0ec72-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0ec72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ec72-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0ec72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ec72-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0ec72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ec72-107">Leia as propriedades e as relações do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0ec72-107">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ec72-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ec72-108">Prerequisites</span></span>
<span data-ttu-id="0ec72-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ec72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ec72-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ec72-111">Permission type</span></span>|<span data-ttu-id="0ec72-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0ec72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ec72-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ec72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ec72-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ec72-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="0ec72-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ec72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ec72-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ec72-116">Not supported.</span></span>|
|<span data-ttu-id="0ec72-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ec72-117">Application</span></span>|<span data-ttu-id="0ec72-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ec72-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ec72-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ec72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ec72-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0ec72-120">Optional query parameters</span></span>
<span data-ttu-id="0ec72-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0ec72-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0ec72-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec72-122">Request headers</span></span>
|<span data-ttu-id="0ec72-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ec72-123">Header</span></span>|<span data-ttu-id="0ec72-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0ec72-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ec72-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ec72-125">Authorization</span></span>|<span data-ttu-id="0ec72-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ec72-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ec72-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0ec72-127">Accept</span></span>|<span data-ttu-id="0ec72-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0ec72-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ec72-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec72-129">Request body</span></span>
<span data-ttu-id="0ec72-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ec72-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ec72-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ec72-131">Response</span></span>
<span data-ttu-id="0ec72-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ec72-132">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ec72-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ec72-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ec72-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec72-134">Request</span></span>
<span data-ttu-id="0ec72-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ec72-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="0ec72-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ec72-136">Response</span></span>
<span data-ttu-id="0ec72-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ec72-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1323

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
    "isBuiltIn": true
  }
}
```





