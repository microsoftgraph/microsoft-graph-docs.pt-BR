---
title: função getAssignedRoleDetails
description: Recupera as definições de função atribuídas e as atribuições de função do usuário atualmente autenticado.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 38b5d704621c0628accf400764a03ba4f422c6aa
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801737"
---
# <a name="getassignedroledetails-function"></a><span data-ttu-id="60b17-103">função getAssignedRoleDetails</span><span class="sxs-lookup"><span data-stu-id="60b17-103">getAssignedRoleDetails function</span></span>

> <span data-ttu-id="60b17-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="60b17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60b17-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60b17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60b17-106">Recupera as definições de função atribuídas e as atribuições de função do usuário atualmente autenticado.</span><span class="sxs-lookup"><span data-stu-id="60b17-106">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60b17-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60b17-107">Prerequisites</span></span>
<span data-ttu-id="60b17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60b17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60b17-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60b17-110">Permission type</span></span>|<span data-ttu-id="60b17-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="60b17-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60b17-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60b17-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60b17-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="60b17-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="60b17-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60b17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60b17-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60b17-115">Not supported.</span></span>|
|<span data-ttu-id="60b17-116">Application</span><span class="sxs-lookup"><span data-stu-id="60b17-116">Application</span></span>|<span data-ttu-id="60b17-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="60b17-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="60b17-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60b17-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleDetails
```

## <a name="request-headers"></a><span data-ttu-id="60b17-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60b17-119">Request headers</span></span>
|<span data-ttu-id="60b17-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60b17-120">Header</span></span>|<span data-ttu-id="60b17-121">Valor</span><span class="sxs-lookup"><span data-stu-id="60b17-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60b17-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="60b17-122">Authorization</span></span>|<span data-ttu-id="60b17-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60b17-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60b17-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60b17-124">Accept</span></span>|<span data-ttu-id="60b17-125">application/json</span><span class="sxs-lookup"><span data-stu-id="60b17-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60b17-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60b17-126">Request body</span></span>
<span data-ttu-id="60b17-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60b17-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60b17-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="60b17-128">Response</span></span>
<span data-ttu-id="60b17-129">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um [deviceAndAppManagementAssignedRoleDetails](../resources/intune-rbac-deviceandappmanagementassignedroledetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60b17-129">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementAssignedRoleDetails](../resources/intune-rbac-deviceandappmanagementassignedroledetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60b17-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60b17-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="60b17-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60b17-131">Request</span></span>
<span data-ttu-id="60b17-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60b17-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleDetails
```

### <a name="response"></a><span data-ttu-id="60b17-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="60b17-133">Response</span></span>
<span data-ttu-id="60b17-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60b17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 245

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
    "roleDefinitionIds": [
      "Role Definition Ids value"
    ],
    "roleAssignmentIds": [
      "Role Assignment Ids value"
    ]
  }
}
```




