---
title: Get roleAssignment
description: Ler propriedades e relações do objeto roleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3800d9d14e106c9e1263106fa9e3aa7619d82bb4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756839"
---
# <a name="get-roleassignment"></a><span data-ttu-id="22775-103">Get roleAssignment</span><span class="sxs-lookup"><span data-stu-id="22775-103">Get roleAssignment</span></span>

<span data-ttu-id="22775-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22775-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22775-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22775-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22775-106">Ler propriedades e relações do objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="22775-106">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22775-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22775-107">Prerequisites</span></span>
<span data-ttu-id="22775-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22775-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22775-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22775-110">Permission type</span></span>|<span data-ttu-id="22775-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22775-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22775-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22775-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22775-113">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22775-113">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="22775-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22775-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22775-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22775-115">Not supported.</span></span>|
|<span data-ttu-id="22775-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22775-116">Application</span></span>|<span data-ttu-id="22775-117">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22775-117">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22775-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22775-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22775-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22775-119">Optional query parameters</span></span>
<span data-ttu-id="22775-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="22775-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22775-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22775-121">Request headers</span></span>
|<span data-ttu-id="22775-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22775-122">Header</span></span>|<span data-ttu-id="22775-123">Valor</span><span class="sxs-lookup"><span data-stu-id="22775-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22775-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="22775-124">Authorization</span></span>|<span data-ttu-id="22775-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22775-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22775-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22775-126">Accept</span></span>|<span data-ttu-id="22775-127">application/json</span><span class="sxs-lookup"><span data-stu-id="22775-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22775-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22775-128">Request body</span></span>
<span data-ttu-id="22775-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22775-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22775-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="22775-130">Response</span></span>
<span data-ttu-id="22775-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22775-131">If successful, this method returns a `200 OK` response code and [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22775-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22775-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="22775-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22775-133">Request</span></span>
<span data-ttu-id="22775-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22775-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="22775-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="22775-135">Response</span></span>
<span data-ttu-id="22775-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22775-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": {
    "@odata.type": "#microsoft.graph.roleAssignment",
    "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
    "displayName": "Display Name value",
    "description": "Description value",
    "resourceScopes": [
      "Resource Scopes value"
    ]
  }
}
```




