---
title: Atualizar managedEBookAssignment
description: Atualizar as propriedades de um objeto managedEBookAssignment.
ms.openlocfilehash: 23a4847b45f9e8c36b92dd1018368d8c102d7b86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006602"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="87e93-103">Atualizar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="87e93-103">Update managedEBookAssignment</span></span>

> <span data-ttu-id="87e93-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="87e93-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87e93-105">Atualizar as propriedades de um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="87e93-105">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87e93-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87e93-106">Prerequisites</span></span>
<span data-ttu-id="87e93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87e93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87e93-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87e93-109">Permission type</span></span>|<span data-ttu-id="87e93-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87e93-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87e93-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87e93-111">Delegated (work or school account)</span></span>|<span data-ttu-id="87e93-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87e93-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="87e93-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87e93-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87e93-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87e93-114">Not supported.</span></span>|
|<span data-ttu-id="87e93-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87e93-115">Application</span></span>|<span data-ttu-id="87e93-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87e93-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87e93-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87e93-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="87e93-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87e93-118">Request headers</span></span>
|<span data-ttu-id="87e93-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87e93-119">Header</span></span>|<span data-ttu-id="87e93-120">Valor</span><span class="sxs-lookup"><span data-stu-id="87e93-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87e93-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="87e93-121">Authorization</span></span>|<span data-ttu-id="87e93-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87e93-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87e93-123">Accept</span><span class="sxs-lookup"><span data-stu-id="87e93-123">Accept</span></span>|<span data-ttu-id="87e93-124">application/json</span><span class="sxs-lookup"><span data-stu-id="87e93-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87e93-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87e93-125">Request body</span></span>
<span data-ttu-id="87e93-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="87e93-126">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="87e93-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="87e93-127">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="87e93-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87e93-128">Property</span></span>|<span data-ttu-id="87e93-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="87e93-129">Type</span></span>|<span data-ttu-id="87e93-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="87e93-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87e93-131">id</span><span class="sxs-lookup"><span data-stu-id="87e93-131">id</span></span>|<span data-ttu-id="87e93-132">String</span><span class="sxs-lookup"><span data-stu-id="87e93-132">String</span></span>|<span data-ttu-id="87e93-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="87e93-133">Key of the entity.</span></span>|
|<span data-ttu-id="87e93-134">destino</span><span class="sxs-lookup"><span data-stu-id="87e93-134">target</span></span>|[<span data-ttu-id="87e93-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="87e93-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="87e93-136">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="87e93-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="87e93-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="87e93-137">installIntent</span></span>|[<span data-ttu-id="87e93-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="87e93-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="87e93-139">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="87e93-139">The install intent for eBook.</span></span> <span data-ttu-id="87e93-140">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="87e93-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="87e93-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="87e93-141">Response</span></span>
<span data-ttu-id="87e93-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87e93-142">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87e93-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87e93-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="87e93-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87e93-144">Request</span></span>
<span data-ttu-id="87e93-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87e93-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="87e93-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="87e93-146">Response</span></span>
<span data-ttu-id="87e93-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87e93-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



