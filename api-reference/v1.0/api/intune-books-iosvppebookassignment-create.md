---
title: Criar iosVppEBookAssignment
description: Criar um novo objeto iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56a560c45be3c1932636c988c11359125469b6b3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013581"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="91e64-103">Criar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="91e64-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="91e64-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91e64-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91e64-105">Criar um novo objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="91e64-105">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91e64-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91e64-106">Prerequisites</span></span>
<span data-ttu-id="91e64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91e64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91e64-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91e64-109">Permission type</span></span>|<span data-ttu-id="91e64-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91e64-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91e64-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91e64-111">Delegated (work or school account)</span></span>|<span data-ttu-id="91e64-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91e64-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="91e64-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91e64-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91e64-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91e64-114">Not supported.</span></span>|
|<span data-ttu-id="91e64-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91e64-115">Application</span></span>|<span data-ttu-id="91e64-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91e64-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91e64-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91e64-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="91e64-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91e64-118">Request headers</span></span>
|<span data-ttu-id="91e64-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91e64-119">Header</span></span>|<span data-ttu-id="91e64-120">Valor</span><span class="sxs-lookup"><span data-stu-id="91e64-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91e64-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="91e64-121">Authorization</span></span>|<span data-ttu-id="91e64-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91e64-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91e64-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91e64-123">Accept</span></span>|<span data-ttu-id="91e64-124">application/json</span><span class="sxs-lookup"><span data-stu-id="91e64-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91e64-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91e64-125">Request body</span></span>
<span data-ttu-id="91e64-126">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="91e64-126">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="91e64-127">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="91e64-127">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="91e64-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91e64-128">Property</span></span>|<span data-ttu-id="91e64-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="91e64-129">Type</span></span>|<span data-ttu-id="91e64-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="91e64-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91e64-131">id</span><span class="sxs-lookup"><span data-stu-id="91e64-131">id</span></span>|<span data-ttu-id="91e64-132">String</span><span class="sxs-lookup"><span data-stu-id="91e64-132">String</span></span>|<span data-ttu-id="91e64-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="91e64-133">Key of the entity.</span></span> <span data-ttu-id="91e64-134">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="91e64-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="91e64-135">destino</span><span class="sxs-lookup"><span data-stu-id="91e64-135">target</span></span>|[<span data-ttu-id="91e64-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="91e64-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="91e64-137">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="91e64-137">The assignment target for eBook.</span></span> <span data-ttu-id="91e64-138">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="91e64-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="91e64-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="91e64-139">installIntent</span></span>|[<span data-ttu-id="91e64-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="91e64-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="91e64-141">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="91e64-141">The install intent for eBook.</span></span> <span data-ttu-id="91e64-142">Herdado de [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="91e64-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="91e64-143">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="91e64-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="91e64-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="91e64-144">Response</span></span>
<span data-ttu-id="91e64-145">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91e64-145">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91e64-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91e64-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="91e64-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91e64-147">Request</span></span>
<span data-ttu-id="91e64-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91e64-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="91e64-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="91e64-149">Response</span></span>
<span data-ttu-id="91e64-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91e64-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "48f05789-5789-48f0-8957-f0488957f048",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



