---
title: Get roleAssignment
description: Ler propriedades e relações do objeto roleAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 50c0acf16575880a99b07bf76f431c573b6f1b4f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512234"
---
# <a name="get-roleassignment"></a><span data-ttu-id="1fd9a-103">Get roleAssignment</span><span class="sxs-lookup"><span data-stu-id="1fd9a-103">Get roleAssignment</span></span>

<span data-ttu-id="1fd9a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fd9a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1fd9a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1fd9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fd9a-106">Ler propriedades e relações do objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1fd9a-106">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fd9a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1fd9a-107">Prerequisites</span></span>
<span data-ttu-id="1fd9a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fd9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fd9a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fd9a-110">Permission type</span></span>|<span data-ttu-id="1fd9a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1fd9a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fd9a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fd9a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1fd9a-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fd9a-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="1fd9a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fd9a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fd9a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fd9a-115">Not supported.</span></span>|
|<span data-ttu-id="1fd9a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fd9a-116">Application</span></span>|<span data-ttu-id="1fd9a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fd9a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fd9a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fd9a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1fd9a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1fd9a-119">Optional query parameters</span></span>
<span data-ttu-id="1fd9a-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1fd9a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1fd9a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fd9a-121">Request headers</span></span>
|<span data-ttu-id="1fd9a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1fd9a-122">Header</span></span>|<span data-ttu-id="1fd9a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1fd9a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fd9a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fd9a-124">Authorization</span></span>|<span data-ttu-id="1fd9a-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fd9a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fd9a-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1fd9a-126">Accept</span></span>|<span data-ttu-id="1fd9a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1fd9a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fd9a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fd9a-128">Request body</span></span>
<span data-ttu-id="1fd9a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1fd9a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fd9a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fd9a-130">Response</span></span>
<span data-ttu-id="1fd9a-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fd9a-131">If successful, this method returns a `200 OK` response code and [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fd9a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1fd9a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fd9a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fd9a-133">Request</span></span>
<span data-ttu-id="1fd9a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fd9a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="1fd9a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fd9a-135">Response</span></span>
<span data-ttu-id="1fd9a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1fd9a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




