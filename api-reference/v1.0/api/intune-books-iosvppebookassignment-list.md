---
title: Listar iosVppEBookAssignments
description: Listar propriedades e relações dos objetos iosVppEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5edcc5cb1c6cd074ac26ca57793d34fe25292b58
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467536"
---
# <a name="list-iosvppebookassignments"></a><span data-ttu-id="c8c16-103">Listar iosVppEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="c8c16-103">List iosVppEBookAssignments</span></span>

<span data-ttu-id="c8c16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8c16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8c16-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8c16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8c16-106">Listar propriedades e relações dos objetos [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c8c16-106">List properties and relationships of the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8c16-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8c16-107">Prerequisites</span></span>
<span data-ttu-id="c8c16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8c16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8c16-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8c16-110">Permission type</span></span>|<span data-ttu-id="c8c16-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c8c16-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8c16-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8c16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8c16-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8c16-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c8c16-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8c16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8c16-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8c16-115">Not supported.</span></span>|
|<span data-ttu-id="c8c16-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8c16-116">Application</span></span>|<span data-ttu-id="c8c16-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8c16-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8c16-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8c16-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c8c16-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8c16-119">Request headers</span></span>
|<span data-ttu-id="c8c16-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8c16-120">Header</span></span>|<span data-ttu-id="c8c16-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c8c16-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8c16-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8c16-122">Authorization</span></span>|<span data-ttu-id="c8c16-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8c16-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8c16-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8c16-124">Accept</span></span>|<span data-ttu-id="c8c16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c8c16-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8c16-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8c16-126">Request body</span></span>
<span data-ttu-id="c8c16-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8c16-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8c16-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8c16-128">Response</span></span>
<span data-ttu-id="c8c16-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8c16-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8c16-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8c16-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8c16-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8c16-131">Request</span></span>
<span data-ttu-id="c8c16-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8c16-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="c8c16-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8c16-133">Response</span></span>
<span data-ttu-id="c8c16-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8c16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 299

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
      "id": "48f05789-5789-48f0-8957-f0488957f048",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```






