---
title: Get iosVppEBookAssignment
description: Ler propriedades e relações do objeto iosVppEBookAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd0f6ce03efe22e34f97bc85ec0a373119715c2b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934254"
---
# <a name="get-iosvppebookassignment"></a><span data-ttu-id="4336b-103">Get iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="4336b-103">Get iosVppEBookAssignment</span></span>

> <span data-ttu-id="4336b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4336b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4336b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4336b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4336b-106">Ler propriedades e relações do objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4336b-106">Read properties and relationships of the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4336b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4336b-107">Prerequisites</span></span>
<span data-ttu-id="4336b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4336b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4336b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4336b-110">Permission type</span></span>|<span data-ttu-id="4336b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4336b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4336b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4336b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4336b-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4336b-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4336b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4336b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4336b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4336b-115">Not supported.</span></span>|
|<span data-ttu-id="4336b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4336b-116">Application</span></span>|<span data-ttu-id="4336b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4336b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4336b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4336b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4336b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4336b-119">Optional query parameters</span></span>
<span data-ttu-id="4336b-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4336b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4336b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4336b-121">Request headers</span></span>
|<span data-ttu-id="4336b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4336b-122">Header</span></span>|<span data-ttu-id="4336b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4336b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4336b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4336b-124">Authorization</span></span>|<span data-ttu-id="4336b-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4336b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4336b-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4336b-126">Accept</span></span>|<span data-ttu-id="4336b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4336b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4336b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4336b-128">Request body</span></span>
<span data-ttu-id="4336b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4336b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4336b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4336b-130">Response</span></span>
<span data-ttu-id="4336b-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4336b-131">If successful, this method returns a `200 OK` response code and [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4336b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4336b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4336b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4336b-133">Request</span></span>
<span data-ttu-id="4336b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4336b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="4336b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4336b-135">Response</span></span>
<span data-ttu-id="4336b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4336b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
    "id": "48f05789-5789-48f0-8957-f0488957f048",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "installIntent": "required"
  }
}
```




