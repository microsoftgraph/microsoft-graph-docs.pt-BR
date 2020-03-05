---
title: Listar deviceAndAppManagementRoleDefinitions
description: Lista propriedades e relações dos objetos deviceAndAppManagementRoleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ddaf05f0c188edf42cfdd2783f61014d000acaf5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459804"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="3d457-103">Listar deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="3d457-103">List deviceAndAppManagementRoleDefinitions</span></span>

<span data-ttu-id="3d457-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3d457-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d457-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3d457-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d457-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3d457-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d457-107">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3d457-107">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d457-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3d457-108">Prerequisites</span></span>
<span data-ttu-id="3d457-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d457-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d457-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d457-111">Permission type</span></span>|<span data-ttu-id="3d457-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3d457-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d457-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d457-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d457-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d457-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="3d457-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d457-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d457-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d457-116">Not supported.</span></span>|
|<span data-ttu-id="3d457-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d457-117">Application</span></span>|<span data-ttu-id="3d457-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d457-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d457-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d457-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="3d457-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d457-120">Request headers</span></span>
|<span data-ttu-id="3d457-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3d457-121">Header</span></span>|<span data-ttu-id="3d457-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3d457-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d457-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d457-123">Authorization</span></span>|<span data-ttu-id="3d457-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d457-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d457-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3d457-125">Accept</span></span>|<span data-ttu-id="3d457-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d457-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d457-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d457-127">Request body</span></span>
<span data-ttu-id="3d457-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d457-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d457-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d457-129">Response</span></span>
<span data-ttu-id="3d457-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d457-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d457-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d457-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d457-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d457-132">Request</span></span>
<span data-ttu-id="3d457-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d457-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="3d457-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d457-134">Response</span></span>
<span data-ttu-id="3d457-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d457-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





