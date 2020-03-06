---
title: Obter deviceAndAppManagementRoleAssignment
description: Ler propriedades de leitura e relações do objeto deviceAndAppManagementRoleAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2f8ce024d1b33996ac4d273c85cdc36a25024673
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512339"
---
# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="24c4d-103">Obter deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="24c4d-103">Get deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="24c4d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24c4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24c4d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="24c4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24c4d-106">Ler propriedades de leitura e relações do objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="24c4d-106">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24c4d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="24c4d-107">Prerequisites</span></span>
<span data-ttu-id="24c4d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24c4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24c4d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24c4d-110">Permission type</span></span>|<span data-ttu-id="24c4d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="24c4d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24c4d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24c4d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24c4d-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="24c4d-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="24c4d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24c4d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24c4d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24c4d-115">Not supported.</span></span>|
|<span data-ttu-id="24c4d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24c4d-116">Application</span></span>|<span data-ttu-id="24c4d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24c4d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24c4d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24c4d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24c4d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="24c4d-119">Optional query parameters</span></span>
<span data-ttu-id="24c4d-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="24c4d-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24c4d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24c4d-121">Request headers</span></span>
|<span data-ttu-id="24c4d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24c4d-122">Header</span></span>|<span data-ttu-id="24c4d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="24c4d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24c4d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="24c4d-124">Authorization</span></span>|<span data-ttu-id="24c4d-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24c4d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24c4d-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="24c4d-126">Accept</span></span>|<span data-ttu-id="24c4d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="24c4d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24c4d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24c4d-128">Request body</span></span>
<span data-ttu-id="24c4d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24c4d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24c4d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="24c4d-130">Response</span></span>
<span data-ttu-id="24c4d-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24c4d-131">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24c4d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24c4d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="24c4d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24c4d-133">Request</span></span>
<span data-ttu-id="24c4d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24c4d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="24c4d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="24c4d-135">Response</span></span>
<span data-ttu-id="24c4d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24c4d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
    "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
    "displayName": "Display Name value",
    "description": "Description value",
    "resourceScopes": [
      "Resource Scopes value"
    ],
    "members": [
      "Members value"
    ]
  }
}
```




