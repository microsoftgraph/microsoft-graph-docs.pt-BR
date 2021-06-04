---
title: Obter deviceAndAppManagementRoleAssignment
description: Ler propriedades de leitura e relações do objeto deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a4d525cb092de8dcfc0bf25457f68823bf0b0730
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52743214"
---
# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="30a30-103">Obter deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="30a30-103">Get deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="30a30-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30a30-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30a30-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30a30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30a30-106">Ler propriedades de leitura e relações do objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="30a30-106">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30a30-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30a30-107">Prerequisites</span></span>
<span data-ttu-id="30a30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30a30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30a30-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30a30-110">Permission type</span></span>|<span data-ttu-id="30a30-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30a30-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30a30-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30a30-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30a30-113">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30a30-113">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="30a30-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30a30-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30a30-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30a30-115">Not supported.</span></span>|
|<span data-ttu-id="30a30-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30a30-116">Application</span></span>|<span data-ttu-id="30a30-117">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30a30-117">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30a30-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30a30-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30a30-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="30a30-119">Optional query parameters</span></span>
<span data-ttu-id="30a30-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="30a30-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30a30-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30a30-121">Request headers</span></span>
|<span data-ttu-id="30a30-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30a30-122">Header</span></span>|<span data-ttu-id="30a30-123">Valor</span><span class="sxs-lookup"><span data-stu-id="30a30-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30a30-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="30a30-124">Authorization</span></span>|<span data-ttu-id="30a30-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30a30-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30a30-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30a30-126">Accept</span></span>|<span data-ttu-id="30a30-127">application/json</span><span class="sxs-lookup"><span data-stu-id="30a30-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30a30-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30a30-128">Request body</span></span>
<span data-ttu-id="30a30-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30a30-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30a30-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="30a30-130">Response</span></span>
<span data-ttu-id="30a30-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30a30-131">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30a30-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30a30-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="30a30-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30a30-133">Request</span></span>
<span data-ttu-id="30a30-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30a30-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="30a30-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="30a30-135">Response</span></span>
<span data-ttu-id="30a30-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30a30-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




