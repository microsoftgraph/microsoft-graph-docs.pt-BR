---
title: Atualizar iosVppEBookAssignment
description: Atualizar as propriedades de um objeto iosVppEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20aa546567bbcc341acd4ff42ab79e5bda4672d5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392530"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="ea093-103">Atualizar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="ea093-103">Update iosVppEBookAssignment</span></span>

<span data-ttu-id="ea093-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea093-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea093-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ea093-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea093-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea093-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea093-107">Atualizar as propriedades de um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea093-107">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea093-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ea093-108">Prerequisites</span></span>
<span data-ttu-id="ea093-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea093-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea093-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea093-111">Permission type</span></span>|<span data-ttu-id="ea093-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ea093-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea093-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea093-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea093-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea093-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ea093-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea093-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea093-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea093-116">Not supported.</span></span>|
|<span data-ttu-id="ea093-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea093-117">Application</span></span>|<span data-ttu-id="ea093-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea093-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea093-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea093-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ea093-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea093-120">Request headers</span></span>
|<span data-ttu-id="ea093-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ea093-121">Header</span></span>|<span data-ttu-id="ea093-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ea093-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea093-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea093-123">Authorization</span></span>|<span data-ttu-id="ea093-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea093-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea093-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ea093-125">Accept</span></span>|<span data-ttu-id="ea093-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea093-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea093-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea093-127">Request body</span></span>
<span data-ttu-id="ea093-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea093-128">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="ea093-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea093-129">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="ea093-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea093-130">Property</span></span>|<span data-ttu-id="ea093-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea093-131">Type</span></span>|<span data-ttu-id="ea093-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea093-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea093-133">id</span><span class="sxs-lookup"><span data-stu-id="ea093-133">id</span></span>|<span data-ttu-id="ea093-134">String</span><span class="sxs-lookup"><span data-stu-id="ea093-134">String</span></span>|<span data-ttu-id="ea093-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ea093-135">Key of the entity.</span></span> <span data-ttu-id="ea093-136">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ea093-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="ea093-137">destino</span><span class="sxs-lookup"><span data-stu-id="ea093-137">target</span></span>|[<span data-ttu-id="ea093-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ea093-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ea093-139">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="ea093-139">The assignment target for eBook.</span></span> <span data-ttu-id="ea093-140">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ea093-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="ea093-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="ea093-141">installIntent</span></span>|[<span data-ttu-id="ea093-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="ea093-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="ea093-143">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="ea093-143">The install intent for eBook.</span></span> <span data-ttu-id="ea093-144">Herdado de [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea093-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="ea093-145">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="ea093-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="ea093-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea093-146">Response</span></span>
<span data-ttu-id="ea093-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea093-147">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea093-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea093-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea093-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea093-149">Request</span></span>
<span data-ttu-id="ea093-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea093-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="ea093-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea093-151">Response</span></span>
<span data-ttu-id="ea093-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea093-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



