---
title: Listar roleDefinitions
description: Listar propriedades e relações dos objetos roleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b202800aef6fc24402478b3de651e2237ffd4d5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899393"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="29037-103">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="29037-103">List roleDefinitions</span></span>

> <span data-ttu-id="29037-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29037-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29037-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29037-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29037-106">Listar propriedades e relações dos objetos [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="29037-106">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29037-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29037-107">Prerequisites</span></span>
<span data-ttu-id="29037-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29037-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29037-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29037-110">Permission type</span></span>|<span data-ttu-id="29037-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29037-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29037-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29037-112">Delegated (work or school account)</span></span>|<span data-ttu-id="29037-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="29037-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="29037-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29037-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29037-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29037-115">Not supported.</span></span>|
|<span data-ttu-id="29037-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29037-116">Application</span></span>|<span data-ttu-id="29037-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29037-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29037-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29037-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="29037-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29037-119">Request headers</span></span>
|<span data-ttu-id="29037-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29037-120">Header</span></span>|<span data-ttu-id="29037-121">Valor</span><span class="sxs-lookup"><span data-stu-id="29037-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29037-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="29037-122">Authorization</span></span>|<span data-ttu-id="29037-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29037-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29037-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29037-124">Accept</span></span>|<span data-ttu-id="29037-125">application/json</span><span class="sxs-lookup"><span data-stu-id="29037-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29037-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29037-126">Request body</span></span>
<span data-ttu-id="29037-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="29037-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29037-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="29037-128">Response</span></span>
<span data-ttu-id="29037-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [roleDefinition](../resources/intune-rbac-roledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29037-129">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29037-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29037-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="29037-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29037-131">Request</span></span>
<span data-ttu-id="29037-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29037-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="29037-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="29037-133">Response</span></span>
<span data-ttu-id="29037-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29037-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1477

{
  "value": [
    {
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
  ]
}
```




