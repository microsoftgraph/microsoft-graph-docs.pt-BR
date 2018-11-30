---
title: Criar managedEBookAssignment
description: Criar um novo objeto managedEBookAssignment.
ms.openlocfilehash: c471362f9f3cfddb9aa2cd3779ac66d28ec5d198
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007000"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="eef18-103">Criar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="eef18-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="eef18-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="eef18-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eef18-105">Criar um novo objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="eef18-105">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eef18-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eef18-106">Prerequisites</span></span>
<span data-ttu-id="eef18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eef18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eef18-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eef18-109">Permission type</span></span>|<span data-ttu-id="eef18-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eef18-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eef18-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eef18-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eef18-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eef18-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eef18-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eef18-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eef18-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eef18-114">Not supported.</span></span>|
|<span data-ttu-id="eef18-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eef18-115">Application</span></span>|<span data-ttu-id="eef18-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eef18-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eef18-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eef18-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="eef18-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eef18-118">Request headers</span></span>
|<span data-ttu-id="eef18-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eef18-119">Header</span></span>|<span data-ttu-id="eef18-120">Valor</span><span class="sxs-lookup"><span data-stu-id="eef18-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eef18-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="eef18-121">Authorization</span></span>|<span data-ttu-id="eef18-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eef18-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eef18-123">Accept</span><span class="sxs-lookup"><span data-stu-id="eef18-123">Accept</span></span>|<span data-ttu-id="eef18-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eef18-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eef18-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eef18-125">Request body</span></span>
<span data-ttu-id="eef18-126">No corpo da solicitação, forneça uma representação JSON do objeto managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="eef18-126">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="eef18-127">A tabela a seguir mostra as propriedades que são necessárias ao criar managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="eef18-127">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="eef18-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eef18-128">Property</span></span>|<span data-ttu-id="eef18-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="eef18-129">Type</span></span>|<span data-ttu-id="eef18-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="eef18-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eef18-131">id</span><span class="sxs-lookup"><span data-stu-id="eef18-131">id</span></span>|<span data-ttu-id="eef18-132">String</span><span class="sxs-lookup"><span data-stu-id="eef18-132">String</span></span>|<span data-ttu-id="eef18-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="eef18-133">Key of the entity.</span></span>|
|<span data-ttu-id="eef18-134">destino</span><span class="sxs-lookup"><span data-stu-id="eef18-134">target</span></span>|[<span data-ttu-id="eef18-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="eef18-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="eef18-136">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="eef18-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="eef18-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="eef18-137">installIntent</span></span>|[<span data-ttu-id="eef18-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="eef18-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="eef18-139">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="eef18-139">The install intent for eBook.</span></span> <span data-ttu-id="eef18-140">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="eef18-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="eef18-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="eef18-141">Response</span></span>
<span data-ttu-id="eef18-142">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eef18-142">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eef18-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eef18-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="eef18-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eef18-144">Request</span></span>
<span data-ttu-id="eef18-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eef18-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="eef18-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="eef18-146">Response</span></span>
<span data-ttu-id="eef18-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eef18-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



