---
title: função getAssignedRoleIdsForLoggedInUser
description: Recupera as definições de função atribuída e as atribuições de função do usuário autenticado no momento.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3385d43eb8ee2680d5e2684ffc21690f627a5034
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823601"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="85995-103">função getAssignedRoleIdsForLoggedInUser</span><span class="sxs-lookup"><span data-stu-id="85995-103">getAssignedRoleIdsForLoggedInUser function</span></span>

> <span data-ttu-id="85995-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="85995-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85995-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="85995-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85995-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="85995-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85995-107">Recupera as definições de função atribuída e as atribuições de função do usuário autenticado no momento.</span><span class="sxs-lookup"><span data-stu-id="85995-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85995-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="85995-108">Prerequisites</span></span>
<span data-ttu-id="85995-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85995-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85995-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85995-111">Permission type</span></span>|<span data-ttu-id="85995-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="85995-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85995-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85995-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85995-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="85995-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="85995-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85995-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85995-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85995-116">Not supported.</span></span>|
|<span data-ttu-id="85995-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85995-117">Application</span></span>|<span data-ttu-id="85995-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85995-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85995-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85995-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="85995-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85995-120">Request headers</span></span>
|<span data-ttu-id="85995-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85995-121">Header</span></span>|<span data-ttu-id="85995-122">Valor</span><span class="sxs-lookup"><span data-stu-id="85995-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85995-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="85995-123">Authorization</span></span>|<span data-ttu-id="85995-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85995-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85995-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="85995-125">Accept</span></span>|<span data-ttu-id="85995-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85995-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85995-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85995-127">Request body</span></span>
<span data-ttu-id="85995-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85995-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85995-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="85995-129">Response</span></span>
<span data-ttu-id="85995-130">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um [deviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85995-130">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85995-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85995-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="85995-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85995-132">Request</span></span>
<span data-ttu-id="85995-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85995-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="85995-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="85995-134">Response</span></span>
<span data-ttu-id="85995-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85995-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





