---
title: Listar managedEBookAssignments
description: Listar propriedades e relações dos objetos managedEBookAssignment.
author: tfitzmac
ms.openlocfilehash: bb4f824c22a8d72a2b083606b8c9367bd15579a0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303532"
---
# <a name="list-managedebookassignments"></a><span data-ttu-id="4c1c2-103">Listar managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="4c1c2-103">List managedEBookAssignments</span></span>

> <span data-ttu-id="4c1c2-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4c1c2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c1c2-105">Listar propriedades e relações dos objetos [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4c1c2-105">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c1c2-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c1c2-106">Prerequisites</span></span>
<span data-ttu-id="4c1c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c1c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c1c2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c1c2-109">Permission type</span></span>|<span data-ttu-id="4c1c2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4c1c2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c1c2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c1c2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4c1c2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c1c2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4c1c2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c1c2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c1c2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c1c2-114">Not supported.</span></span>|
|<span data-ttu-id="4c1c2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c1c2-115">Application</span></span>|<span data-ttu-id="4c1c2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c1c2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c1c2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c1c2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4c1c2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c1c2-118">Request headers</span></span>
|<span data-ttu-id="4c1c2-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c1c2-119">Header</span></span>|<span data-ttu-id="4c1c2-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4c1c2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c1c2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c1c2-121">Authorization</span></span>|<span data-ttu-id="4c1c2-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c1c2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c1c2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4c1c2-123">Accept</span></span>|<span data-ttu-id="4c1c2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4c1c2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c1c2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c1c2-125">Request body</span></span>
<span data-ttu-id="4c1c2-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c1c2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c1c2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c1c2-127">Response</span></span>
<span data-ttu-id="4c1c2-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c1c2-128">If successful, this method returns a `200 OK` response code and a collection of [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c1c2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c1c2-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c1c2-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c1c2-130">Request</span></span>
<span data-ttu-id="4c1c2-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c1c2-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="4c1c2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c1c2-132">Response</span></span>
<span data-ttu-id="4c1c2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c1c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



