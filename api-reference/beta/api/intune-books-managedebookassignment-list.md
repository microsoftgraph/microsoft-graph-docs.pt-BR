---
title: Listar managedEBookAssignments
description: Listar propriedades e relações dos objetos managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3ac6468147016e9312a175bf389cdb4a74e8a156
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685314"
---
# <a name="list-managedebookassignments"></a><span data-ttu-id="b03ad-103">Listar managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="b03ad-103">List managedEBookAssignments</span></span>

<span data-ttu-id="b03ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b03ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b03ad-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b03ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b03ad-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b03ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b03ad-107">Listar propriedades e relações dos objetos [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b03ad-107">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b03ad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b03ad-108">Prerequisites</span></span>
<span data-ttu-id="b03ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b03ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b03ad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b03ad-111">Permission type</span></span>|<span data-ttu-id="b03ad-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b03ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b03ad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b03ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b03ad-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b03ad-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b03ad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b03ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b03ad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b03ad-116">Not supported.</span></span>|
|<span data-ttu-id="b03ad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b03ad-117">Application</span></span>|<span data-ttu-id="b03ad-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b03ad-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b03ad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b03ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b03ad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b03ad-120">Request headers</span></span>
|<span data-ttu-id="b03ad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b03ad-121">Header</span></span>|<span data-ttu-id="b03ad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b03ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b03ad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b03ad-123">Authorization</span></span>|<span data-ttu-id="b03ad-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b03ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b03ad-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b03ad-125">Accept</span></span>|<span data-ttu-id="b03ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b03ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b03ad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b03ad-127">Request body</span></span>
<span data-ttu-id="b03ad-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b03ad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b03ad-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b03ad-129">Response</span></span>
<span data-ttu-id="b03ad-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b03ad-130">If successful, this method returns a `200 OK` response code and a collection of [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b03ad-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b03ad-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b03ad-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b03ad-132">Request</span></span>
<span data-ttu-id="b03ad-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b03ad-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="b03ad-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b03ad-134">Response</span></span>
<span data-ttu-id="b03ad-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b03ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





