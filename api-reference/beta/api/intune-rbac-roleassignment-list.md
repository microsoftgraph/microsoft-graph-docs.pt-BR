---
title: Listar roleAssignments
description: Listar propriedades e relações de objeto de roleAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ea9cf864264deb6b7f1e9bb206ef3ccb4776365
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988528"
---
# <a name="list-roleassignments"></a><span data-ttu-id="05ebe-103">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="05ebe-103">List roleAssignments</span></span>

> <span data-ttu-id="05ebe-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="05ebe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05ebe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05ebe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05ebe-106">Listar propriedades e relações de objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="05ebe-106">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05ebe-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05ebe-107">Prerequisites</span></span>
<span data-ttu-id="05ebe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05ebe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05ebe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05ebe-110">Permission type</span></span>|<span data-ttu-id="05ebe-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05ebe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05ebe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05ebe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05ebe-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="05ebe-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="05ebe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05ebe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05ebe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05ebe-115">Not supported.</span></span>|
|<span data-ttu-id="05ebe-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05ebe-116">Application</span></span>|<span data-ttu-id="05ebe-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05ebe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05ebe-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05ebe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="05ebe-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05ebe-119">Request headers</span></span>
|<span data-ttu-id="05ebe-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05ebe-120">Header</span></span>|<span data-ttu-id="05ebe-121">Valor</span><span class="sxs-lookup"><span data-stu-id="05ebe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05ebe-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="05ebe-122">Authorization</span></span>|<span data-ttu-id="05ebe-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05ebe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05ebe-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05ebe-124">Accept</span></span>|<span data-ttu-id="05ebe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="05ebe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05ebe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05ebe-126">Request body</span></span>
<span data-ttu-id="05ebe-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="05ebe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05ebe-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="05ebe-128">Response</span></span>
<span data-ttu-id="05ebe-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05ebe-129">If successful, this method returns a `200 OK` response code and a collection of [roleAssignment](../resources/intune-rbac-roleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05ebe-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05ebe-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="05ebe-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05ebe-131">Request</span></span>
<span data-ttu-id="05ebe-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05ebe-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

### <a name="response"></a><span data-ttu-id="05ebe-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="05ebe-133">Response</span></span>
<span data-ttu-id="05ebe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05ebe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 403

{
  "value": [
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
  ]
}
```





