---
title: função getAssignedRoleIdsForLoggedInUser
description: Recupera as definições de função atribuídas e as atribuições de função do usuário atualmente autenticado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6790d5121c8c3eced7ee0a5ea769469b8b9eaee5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390172"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="8ae7e-103">função getAssignedRoleIdsForLoggedInUser</span><span class="sxs-lookup"><span data-stu-id="8ae7e-103">getAssignedRoleIdsForLoggedInUser function</span></span>

<span data-ttu-id="8ae7e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ae7e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ae7e-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8ae7e-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8ae7e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8ae7e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ae7e-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ae7e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ae7e-108">Recupera as definições de função atribuídas e as atribuições de função do usuário atualmente autenticado.</span><span class="sxs-lookup"><span data-stu-id="8ae7e-108">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8ae7e-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8ae7e-109">Prerequisites</span></span>
<span data-ttu-id="8ae7e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ae7e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ae7e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ae7e-112">Permission type</span></span>|<span data-ttu-id="8ae7e-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8ae7e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ae7e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ae7e-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8ae7e-115">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="8ae7e-115">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="8ae7e-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ae7e-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="8ae7e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ae7e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ae7e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ae7e-118">Not supported.</span></span>|
|<span data-ttu-id="8ae7e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ae7e-119">Application</span></span>||
| <span data-ttu-id="8ae7e-120">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="8ae7e-120">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="8ae7e-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ae7e-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="8ae7e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ae7e-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="8ae7e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ae7e-123">Request headers</span></span>
|<span data-ttu-id="8ae7e-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ae7e-124">Header</span></span>|<span data-ttu-id="8ae7e-125">Valor</span><span class="sxs-lookup"><span data-stu-id="8ae7e-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ae7e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ae7e-126">Authorization</span></span>|<span data-ttu-id="8ae7e-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ae7e-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ae7e-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8ae7e-128">Accept</span></span>|<span data-ttu-id="8ae7e-129">application/json</span><span class="sxs-lookup"><span data-stu-id="8ae7e-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ae7e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ae7e-130">Request body</span></span>
<span data-ttu-id="8ae7e-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ae7e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ae7e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ae7e-132">Response</span></span>
<span data-ttu-id="8ae7e-133">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um **deviceAndAppManagementAssignedRoleId** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ae7e-133">If successful, this function returns a `200 OK` response code and a **deviceAndAppManagementAssignedRoleId** in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ae7e-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ae7e-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ae7e-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ae7e-135">Request</span></span>
<span data-ttu-id="8ae7e-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ae7e-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="8ae7e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ae7e-137">Response</span></span>
<span data-ttu-id="8ae7e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ae7e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











