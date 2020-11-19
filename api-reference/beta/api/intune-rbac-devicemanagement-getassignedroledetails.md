---
title: função getAssignedRoleDetails
description: Recupera as definições de função atribuídas e as atribuições de função do usuário atualmente autenticado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8c4c1ce286d5d5fd79ab7cbf6df2476105ad5bcc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49304900"
---
# <a name="getassignedroledetails-function"></a><span data-ttu-id="f5412-103">função getAssignedRoleDetails</span><span class="sxs-lookup"><span data-stu-id="f5412-103">getAssignedRoleDetails function</span></span>

<span data-ttu-id="f5412-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5412-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5412-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f5412-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5412-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f5412-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5412-107">Recupera as definições de função atribuídas e as atribuições de função do usuário atualmente autenticado.</span><span class="sxs-lookup"><span data-stu-id="f5412-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5412-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5412-108">Prerequisites</span></span>
<span data-ttu-id="f5412-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5412-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5412-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5412-111">Permission type</span></span>|<span data-ttu-id="f5412-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f5412-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5412-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5412-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5412-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5412-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="f5412-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5412-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5412-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5412-116">Not supported.</span></span>|
|<span data-ttu-id="f5412-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5412-117">Application</span></span>|<span data-ttu-id="f5412-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5412-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5412-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5412-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleDetails
```

## <a name="request-headers"></a><span data-ttu-id="f5412-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5412-120">Request headers</span></span>
|<span data-ttu-id="f5412-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5412-121">Header</span></span>|<span data-ttu-id="f5412-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f5412-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5412-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5412-123">Authorization</span></span>|<span data-ttu-id="f5412-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5412-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5412-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5412-125">Accept</span></span>|<span data-ttu-id="f5412-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5412-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5412-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5412-127">Request body</span></span>
<span data-ttu-id="f5412-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5412-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5412-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5412-129">Response</span></span>
<span data-ttu-id="f5412-130">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um [deviceAndAppManagementAssignedRoleDetails](../resources/intune-rbac-deviceandappmanagementassignedroledetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5412-130">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementAssignedRoleDetails](../resources/intune-rbac-deviceandappmanagementassignedroledetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5412-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5412-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5412-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5412-132">Request</span></span>
<span data-ttu-id="f5412-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5412-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleDetails
```

### <a name="response"></a><span data-ttu-id="f5412-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5412-134">Response</span></span>
<span data-ttu-id="f5412-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5412-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




