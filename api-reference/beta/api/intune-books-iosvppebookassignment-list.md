---
title: Listar iosVppEBookAssignments
description: Listar propriedades e relações dos objetos iosVppEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 54704ee6fcdffdbf9a33ebb5b6e2a090647b8df3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975651"
---
# <a name="list-iosvppebookassignments"></a><span data-ttu-id="edb66-103">Listar iosVppEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="edb66-103">List iosVppEBookAssignments</span></span>

<span data-ttu-id="edb66-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edb66-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edb66-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="edb66-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edb66-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="edb66-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edb66-107">Listar propriedades e relações dos objetos [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="edb66-107">List properties and relationships of the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="edb66-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="edb66-108">Prerequisites</span></span>
<span data-ttu-id="edb66-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edb66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edb66-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="edb66-111">Permission type</span></span>|<span data-ttu-id="edb66-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="edb66-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edb66-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="edb66-113">Delegated (work or school account)</span></span>|<span data-ttu-id="edb66-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="edb66-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="edb66-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="edb66-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edb66-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="edb66-116">Not supported.</span></span>|
|<span data-ttu-id="edb66-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="edb66-117">Application</span></span>|<span data-ttu-id="edb66-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="edb66-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="edb66-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="edb66-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="edb66-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="edb66-120">Request headers</span></span>
|<span data-ttu-id="edb66-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="edb66-121">Header</span></span>|<span data-ttu-id="edb66-122">Valor</span><span class="sxs-lookup"><span data-stu-id="edb66-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edb66-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="edb66-123">Authorization</span></span>|<span data-ttu-id="edb66-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="edb66-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edb66-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="edb66-125">Accept</span></span>|<span data-ttu-id="edb66-126">application/json</span><span class="sxs-lookup"><span data-stu-id="edb66-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edb66-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="edb66-127">Request body</span></span>
<span data-ttu-id="edb66-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="edb66-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edb66-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="edb66-129">Response</span></span>
<span data-ttu-id="edb66-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="edb66-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edb66-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="edb66-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="edb66-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="edb66-132">Request</span></span>
<span data-ttu-id="edb66-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="edb66-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="edb66-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="edb66-134">Response</span></span>
<span data-ttu-id="edb66-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="edb66-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 474

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
      "id": "48f05789-5789-48f0-8957-f0488957f048",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "installIntent": "required"
    }
  ]
}
```






