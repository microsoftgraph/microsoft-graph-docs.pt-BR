---
title: Listar managedEBookAssignments
description: Listar propriedades e relações dos objetos managedEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f8cfe21611e2c656390c7c2609c9bca0c997913a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258874"
---
# <a name="list-managedebookassignments"></a><span data-ttu-id="86fda-103">Listar managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="86fda-103">List managedEBookAssignments</span></span>

> <span data-ttu-id="86fda-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86fda-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86fda-105">Listar propriedades e relações dos objetos [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="86fda-105">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86fda-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86fda-106">Prerequisites</span></span>
<span data-ttu-id="86fda-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="86fda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="86fda-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86fda-109">Permission type</span></span>|<span data-ttu-id="86fda-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86fda-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86fda-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86fda-111">Delegated (work or school account)</span></span>|<span data-ttu-id="86fda-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="86fda-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="86fda-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86fda-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86fda-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86fda-114">Not supported.</span></span>|
|<span data-ttu-id="86fda-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86fda-115">Application</span></span>|<span data-ttu-id="86fda-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86fda-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86fda-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86fda-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="86fda-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86fda-118">Request headers</span></span>
|<span data-ttu-id="86fda-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86fda-119">Header</span></span>|<span data-ttu-id="86fda-120">Valor</span><span class="sxs-lookup"><span data-stu-id="86fda-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86fda-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="86fda-121">Authorization</span></span>|<span data-ttu-id="86fda-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86fda-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86fda-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86fda-123">Accept</span></span>|<span data-ttu-id="86fda-124">application/json</span><span class="sxs-lookup"><span data-stu-id="86fda-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86fda-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86fda-125">Request body</span></span>
<span data-ttu-id="86fda-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86fda-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86fda-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="86fda-127">Response</span></span>
<span data-ttu-id="86fda-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86fda-128">If successful, this method returns a `200 OK` response code and a collection of [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86fda-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86fda-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="86fda-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86fda-130">Request</span></span>
<span data-ttu-id="86fda-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86fda-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="86fda-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="86fda-132">Response</span></span>
<span data-ttu-id="86fda-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86fda-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 300

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```



