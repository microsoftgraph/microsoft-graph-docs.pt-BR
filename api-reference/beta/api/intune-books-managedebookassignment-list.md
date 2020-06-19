---
title: Listar managedEBookAssignments
description: Listar propriedades e relações dos objetos managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b5ce010bd629ff0c2bb149bc30a022f642494bcd
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793189"
---
# <a name="list-managedebookassignments"></a><span data-ttu-id="3623c-103">Listar managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="3623c-103">List managedEBookAssignments</span></span>

<span data-ttu-id="3623c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3623c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3623c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3623c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3623c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3623c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3623c-107">Listar propriedades e relações dos objetos [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3623c-107">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3623c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3623c-108">Prerequisites</span></span>
<span data-ttu-id="3623c-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3623c-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3623c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3623c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3623c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3623c-111">Permission type</span></span>|<span data-ttu-id="3623c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3623c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3623c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3623c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3623c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3623c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3623c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3623c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3623c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3623c-116">Not supported.</span></span>|
|<span data-ttu-id="3623c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3623c-117">Application</span></span>|<span data-ttu-id="3623c-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3623c-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3623c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3623c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="3623c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3623c-120">Request headers</span></span>
|<span data-ttu-id="3623c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3623c-121">Header</span></span>|<span data-ttu-id="3623c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3623c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3623c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3623c-123">Authorization</span></span>|<span data-ttu-id="3623c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3623c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3623c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3623c-125">Accept</span></span>|<span data-ttu-id="3623c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3623c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3623c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3623c-127">Request body</span></span>
<span data-ttu-id="3623c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3623c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3623c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3623c-129">Response</span></span>
<span data-ttu-id="3623c-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3623c-130">If successful, this method returns a `200 OK` response code and a collection of [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3623c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3623c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3623c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3623c-132">Request</span></span>
<span data-ttu-id="3623c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3623c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="3623c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3623c-134">Response</span></span>
<span data-ttu-id="3623c-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="3623c-135">Here is an example of the response.</span></span> <span data-ttu-id="3623c-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="3623c-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3623c-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3623c-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 469

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "installIntent": "required"
    }
  ]
}
```



