---
title: função getAssignedRoleIdsForLoggedInUser
description: Recupera as definições de função atribuídas e as atribuições de função do usuário atualmente autenticado.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c7f7596835d0ada69a8bcefdc62781ba938d4938
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939981"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="f031b-103">função getAssignedRoleIdsForLoggedInUser</span><span class="sxs-lookup"><span data-stu-id="f031b-103">getAssignedRoleIdsForLoggedInUser function</span></span>

> <span data-ttu-id="f031b-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f031b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f031b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f031b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f031b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f031b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f031b-107">Recupera as definições de função atribuídas e as atribuições de função do usuário atualmente autenticado.</span><span class="sxs-lookup"><span data-stu-id="f031b-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f031b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f031b-108">Prerequisites</span></span>
<span data-ttu-id="f031b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f031b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f031b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f031b-111">Permission type</span></span>|<span data-ttu-id="f031b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f031b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f031b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f031b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f031b-114">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="f031b-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="f031b-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="f031b-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="f031b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f031b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f031b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f031b-117">Not supported.</span></span>|
|<span data-ttu-id="f031b-118">Application</span><span class="sxs-lookup"><span data-stu-id="f031b-118">Application</span></span>||
| <span data-ttu-id="f031b-119">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="f031b-119">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="f031b-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="f031b-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="f031b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f031b-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="f031b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f031b-122">Request headers</span></span>
|<span data-ttu-id="f031b-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f031b-123">Header</span></span>|<span data-ttu-id="f031b-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f031b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f031b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f031b-125">Authorization</span></span>|<span data-ttu-id="f031b-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f031b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f031b-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f031b-127">Accept</span></span>|<span data-ttu-id="f031b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f031b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f031b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f031b-129">Request body</span></span>
<span data-ttu-id="f031b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f031b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f031b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f031b-131">Response</span></span>
<span data-ttu-id="f031b-132">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um **deviceAndAppManagementAssignedRoleId** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f031b-132">If successful, this function returns a `200 OK` response code and a **deviceAndAppManagementAssignedRoleId** in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f031b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f031b-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="f031b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f031b-134">Request</span></span>
<span data-ttu-id="f031b-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f031b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="f031b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f031b-136">Response</span></span>
<span data-ttu-id="f031b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f031b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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













