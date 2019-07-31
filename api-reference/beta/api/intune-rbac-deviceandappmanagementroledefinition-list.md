---
title: Listar deviceAndAppManagementRoleDefinitions
description: Lista propriedades e relações dos objetos deviceAndAppManagementRoleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3a36a6dd45f1c022438c2430886f55534c8ac26d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35980146"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="b8a4b-103">Listar deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="b8a4b-103">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="b8a4b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b8a4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8a4b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8a4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8a4b-106">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b8a4b-106">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8a4b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8a4b-107">Prerequisites</span></span>
<span data-ttu-id="b8a4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8a4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8a4b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8a4b-110">Permission type</span></span>|<span data-ttu-id="b8a4b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b8a4b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8a4b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8a4b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b8a4b-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8a4b-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="b8a4b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8a4b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8a4b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8a4b-115">Not supported.</span></span>|
|<span data-ttu-id="b8a4b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8a4b-116">Application</span></span>|<span data-ttu-id="b8a4b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8a4b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8a4b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8a4b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="b8a4b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8a4b-119">Request headers</span></span>
|<span data-ttu-id="b8a4b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8a4b-120">Header</span></span>|<span data-ttu-id="b8a4b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b8a4b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8a4b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8a4b-122">Authorization</span></span>|<span data-ttu-id="b8a4b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8a4b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8a4b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8a4b-124">Accept</span></span>|<span data-ttu-id="b8a4b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b8a4b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8a4b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8a4b-126">Request body</span></span>
<span data-ttu-id="b8a4b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8a4b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8a4b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8a4b-128">Response</span></span>
<span data-ttu-id="b8a4b-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8a4b-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8a4b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8a4b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8a4b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8a4b-131">Request</span></span>
<span data-ttu-id="b8a4b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8a4b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="b8a4b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8a4b-133">Response</span></span>
<span data-ttu-id="b8a4b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8a4b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1499

{
  "value": [
    {
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
  ]
}
```





