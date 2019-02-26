---
title: Listar deviceAndAppManagementRoleDefinitions
description: Lista propriedades e relações dos objetos deviceAndAppManagementRoleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b96f69854e0916aa70101767eff61aa8cbdd5033
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253089"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="c8840-103">Listar deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="c8840-103">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="c8840-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8840-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8840-105">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c8840-105">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8840-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8840-106">Prerequisites</span></span>
<span data-ttu-id="c8840-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c8840-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c8840-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8840-109">Permission type</span></span>|<span data-ttu-id="c8840-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c8840-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8840-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8840-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c8840-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8840-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="c8840-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8840-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8840-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8840-114">Not supported.</span></span>|
|<span data-ttu-id="c8840-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8840-115">Application</span></span>|<span data-ttu-id="c8840-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8840-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8840-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8840-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="c8840-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8840-118">Request headers</span></span>
|<span data-ttu-id="c8840-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8840-119">Header</span></span>|<span data-ttu-id="c8840-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c8840-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8840-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8840-121">Authorization</span></span>|<span data-ttu-id="c8840-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8840-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8840-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8840-123">Accept</span></span>|<span data-ttu-id="c8840-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c8840-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8840-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8840-125">Request body</span></span>
<span data-ttu-id="c8840-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8840-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8840-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8840-127">Response</span></span>
<span data-ttu-id="c8840-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8840-128">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8840-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8840-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8840-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8840-130">Request</span></span>
<span data-ttu-id="c8840-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8840-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="c8840-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8840-132">Response</span></span>
<span data-ttu-id="c8840-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8840-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 768

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
      "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
      "displayName": "Display Name value",
      "description": "Description value",
      "rolePermissions": [
        {
          "@odata.type": "microsoft.graph.rolePermission",
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
      "isBuiltIn": true
    }
  ]
}
```



