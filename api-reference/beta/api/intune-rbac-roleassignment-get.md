---
title: Get roleAssignment
description: Ler propriedades e relações do objeto roleAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8cfcddd6c82035c4583d0ce246888e2eb8512b6f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403389"
---
# <a name="get-roleassignment"></a><span data-ttu-id="42237-103">Get roleAssignment</span><span class="sxs-lookup"><span data-stu-id="42237-103">Get roleAssignment</span></span>

> <span data-ttu-id="42237-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="42237-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="42237-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="42237-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42237-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="42237-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42237-107">Ler propriedades e relações do objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="42237-107">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42237-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42237-108">Prerequisites</span></span>
<span data-ttu-id="42237-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="42237-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="42237-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42237-111">Permission type</span></span>|<span data-ttu-id="42237-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42237-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42237-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42237-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42237-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="42237-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="42237-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42237-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42237-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42237-116">Not supported.</span></span>|
|<span data-ttu-id="42237-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42237-117">Application</span></span>|<span data-ttu-id="42237-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42237-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42237-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42237-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42237-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="42237-120">Optional query parameters</span></span>
<span data-ttu-id="42237-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="42237-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42237-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42237-122">Request headers</span></span>
|<span data-ttu-id="42237-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42237-123">Header</span></span>|<span data-ttu-id="42237-124">Valor</span><span class="sxs-lookup"><span data-stu-id="42237-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42237-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="42237-125">Authorization</span></span>|<span data-ttu-id="42237-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42237-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42237-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42237-127">Accept</span></span>|<span data-ttu-id="42237-128">application/json</span><span class="sxs-lookup"><span data-stu-id="42237-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42237-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42237-129">Request body</span></span>
<span data-ttu-id="42237-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42237-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42237-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="42237-131">Response</span></span>
<span data-ttu-id="42237-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42237-132">If successful, this method returns a `200 OK` response code and [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42237-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42237-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="42237-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42237-134">Request</span></span>
<span data-ttu-id="42237-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42237-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="42237-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="42237-136">Response</span></span>
<span data-ttu-id="42237-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42237-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 367

{
  "value": {
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
}
```




