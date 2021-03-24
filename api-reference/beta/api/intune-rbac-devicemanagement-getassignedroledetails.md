---
title: função getAssignedRoleDetails
description: Recupera as definições de função atribuídas e as atribuições de função do usuário autenticado no momento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e50ae596bd18d4d20b09da87018539c4ba598602
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148488"
---
# <a name="getassignedroledetails-function"></a><span data-ttu-id="8b645-103">função getAssignedRoleDetails</span><span class="sxs-lookup"><span data-stu-id="8b645-103">getAssignedRoleDetails function</span></span>

<span data-ttu-id="8b645-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b645-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b645-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8b645-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b645-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8b645-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b645-107">Recupera as definições de função atribuídas e as atribuições de função do usuário autenticado no momento.</span><span class="sxs-lookup"><span data-stu-id="8b645-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b645-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8b645-108">Prerequisites</span></span>
<span data-ttu-id="8b645-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b645-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b645-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b645-111">Permission type</span></span>|<span data-ttu-id="8b645-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b645-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b645-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b645-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b645-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b645-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="8b645-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b645-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b645-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b645-116">Not supported.</span></span>|
|<span data-ttu-id="8b645-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b645-117">Application</span></span>|<span data-ttu-id="8b645-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b645-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b645-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b645-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleDetails
```

## <a name="request-headers"></a><span data-ttu-id="8b645-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b645-120">Request headers</span></span>
|<span data-ttu-id="8b645-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8b645-121">Header</span></span>|<span data-ttu-id="8b645-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8b645-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b645-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b645-123">Authorization</span></span>|<span data-ttu-id="8b645-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b645-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b645-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8b645-125">Accept</span></span>|<span data-ttu-id="8b645-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b645-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b645-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b645-127">Request body</span></span>
<span data-ttu-id="8b645-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8b645-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b645-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b645-129">Response</span></span>
<span data-ttu-id="8b645-130">Se tiver êxito, essa função retornará um código de resposta e um `200 OK` [deviceAndAppManagementAssignedRoleDetails](../resources/intune-rbac-deviceandappmanagementassignedroledetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b645-130">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementAssignedRoleDetails](../resources/intune-rbac-deviceandappmanagementassignedroledetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b645-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b645-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b645-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b645-132">Request</span></span>
<span data-ttu-id="8b645-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b645-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleDetails
```

### <a name="response"></a><span data-ttu-id="8b645-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b645-134">Response</span></span>
<span data-ttu-id="8b645-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8b645-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




