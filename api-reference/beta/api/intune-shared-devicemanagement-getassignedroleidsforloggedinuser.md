---
title: função getAssignedRoleIdsForLoggedInUser
description: Recupera as definições de função atribuída e as atribuições de função do usuário autenticado no momento.
author: tfitzmac
ms.openlocfilehash: 0e9cf6e45c0f7ce7e321d746d12648a598109df5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331091"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="27f65-103">função getAssignedRoleIdsForLoggedInUser</span><span class="sxs-lookup"><span data-stu-id="27f65-103">getAssignedRoleIdsForLoggedInUser function</span></span>

> <span data-ttu-id="27f65-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="27f65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27f65-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="27f65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27f65-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="27f65-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27f65-107">Recupera as definições de função atribuída e as atribuições de função do usuário autenticado no momento.</span><span class="sxs-lookup"><span data-stu-id="27f65-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27f65-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27f65-108">Prerequisites</span></span>
<span data-ttu-id="27f65-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27f65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27f65-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27f65-111">Permission type</span></span>|<span data-ttu-id="27f65-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27f65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27f65-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27f65-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="27f65-114">&nbsp;&nbsp; **O controle de acesso baseado em função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="27f65-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="27f65-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="27f65-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="27f65-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27f65-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27f65-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27f65-117">Not supported.</span></span>|
|<span data-ttu-id="27f65-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27f65-118">Application</span></span>|<span data-ttu-id="27f65-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27f65-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27f65-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27f65-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="27f65-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27f65-121">Request headers</span></span>
|<span data-ttu-id="27f65-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27f65-122">Header</span></span>|<span data-ttu-id="27f65-123">Valor</span><span class="sxs-lookup"><span data-stu-id="27f65-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27f65-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="27f65-124">Authorization</span></span>|<span data-ttu-id="27f65-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27f65-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27f65-126">Accept</span><span class="sxs-lookup"><span data-stu-id="27f65-126">Accept</span></span>|<span data-ttu-id="27f65-127">application/json</span><span class="sxs-lookup"><span data-stu-id="27f65-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27f65-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27f65-128">Request body</span></span>
<span data-ttu-id="27f65-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27f65-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27f65-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="27f65-130">Response</span></span>
<span data-ttu-id="27f65-131">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um [deviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27f65-131">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27f65-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27f65-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="27f65-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27f65-133">Request</span></span>
<span data-ttu-id="27f65-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27f65-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="27f65-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="27f65-135">Response</span></span>
<span data-ttu-id="27f65-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27f65-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleIds",
    "roleDefinitionIds": [
      "df52f163-f163-df52-63f1-52df63f152df"
    ],
    "roleAssignmentIds": [
      "1f35d53d-d53d-1f35-3dd5-351f3dd5351f"
    ]
  }
}
```





