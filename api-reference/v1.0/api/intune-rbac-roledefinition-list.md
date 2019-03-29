---
title: Listar roleDefinitions
description: Listar propriedades e relações dos objetos roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4df05098fccbc74056a0e10516b573dfce0ca141
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976453"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="7bc48-103">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="7bc48-103">List roleDefinitions</span></span>

> <span data-ttu-id="7bc48-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7bc48-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bc48-105">Listar propriedades e relações dos objetos [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7bc48-105">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7bc48-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7bc48-106">Prerequisites</span></span>
<span data-ttu-id="7bc48-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bc48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bc48-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bc48-109">Permission type</span></span>|<span data-ttu-id="7bc48-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7bc48-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bc48-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bc48-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7bc48-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7bc48-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="7bc48-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bc48-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bc48-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bc48-114">Not supported.</span></span>|
|<span data-ttu-id="7bc48-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bc48-115">Application</span></span>|<span data-ttu-id="7bc48-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bc48-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bc48-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bc48-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="7bc48-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bc48-118">Request headers</span></span>
|<span data-ttu-id="7bc48-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7bc48-119">Header</span></span>|<span data-ttu-id="7bc48-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7bc48-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bc48-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bc48-121">Authorization</span></span>|<span data-ttu-id="7bc48-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bc48-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bc48-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7bc48-123">Accept</span></span>|<span data-ttu-id="7bc48-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7bc48-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bc48-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bc48-125">Request body</span></span>
<span data-ttu-id="7bc48-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7bc48-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bc48-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bc48-127">Response</span></span>
<span data-ttu-id="7bc48-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [roleDefinition](../resources/intune-rbac-roledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7bc48-128">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bc48-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7bc48-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bc48-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bc48-130">Request</span></span>
<span data-ttu-id="7bc48-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7bc48-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="7bc48-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bc48-132">Response</span></span>
<span data-ttu-id="7bc48-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7bc48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 746

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleDefinition",
      "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
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



