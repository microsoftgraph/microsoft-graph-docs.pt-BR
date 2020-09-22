---
title: Atualizar managedEBookAssignment
description: Atualizar as propriedades de um objeto managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 25088846f815054501f1ee0b87265a17f34ea014
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48077818"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="aa776-103">Atualizar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="aa776-103">Update managedEBookAssignment</span></span>

<span data-ttu-id="aa776-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa776-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa776-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa776-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa776-106">Atualizar as propriedades de um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="aa776-106">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa776-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aa776-107">Prerequisites</span></span>
<span data-ttu-id="aa776-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa776-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa776-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa776-110">Permission type</span></span>|<span data-ttu-id="aa776-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aa776-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa776-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa776-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aa776-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa776-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aa776-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa776-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa776-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa776-115">Not supported.</span></span>|
|<span data-ttu-id="aa776-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa776-116">Application</span></span>|<span data-ttu-id="aa776-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa776-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa776-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa776-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="aa776-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa776-119">Request headers</span></span>
|<span data-ttu-id="aa776-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa776-120">Header</span></span>|<span data-ttu-id="aa776-121">Valor</span><span class="sxs-lookup"><span data-stu-id="aa776-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa776-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa776-122">Authorization</span></span>|<span data-ttu-id="aa776-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa776-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa776-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aa776-124">Accept</span></span>|<span data-ttu-id="aa776-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aa776-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa776-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa776-126">Request body</span></span>
<span data-ttu-id="aa776-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="aa776-127">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="aa776-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="aa776-128">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="aa776-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa776-129">Property</span></span>|<span data-ttu-id="aa776-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa776-130">Type</span></span>|<span data-ttu-id="aa776-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa776-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa776-132">id</span><span class="sxs-lookup"><span data-stu-id="aa776-132">id</span></span>|<span data-ttu-id="aa776-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa776-133">String</span></span>|<span data-ttu-id="aa776-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aa776-134">Key of the entity.</span></span>|
|<span data-ttu-id="aa776-135">destino</span><span class="sxs-lookup"><span data-stu-id="aa776-135">target</span></span>|[<span data-ttu-id="aa776-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="aa776-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="aa776-137">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="aa776-137">The assignment target for eBook.</span></span>|
|<span data-ttu-id="aa776-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="aa776-138">installIntent</span></span>|[<span data-ttu-id="aa776-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="aa776-139">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="aa776-140">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="aa776-140">The install intent for eBook.</span></span> <span data-ttu-id="aa776-141">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="aa776-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="aa776-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa776-142">Response</span></span>
<span data-ttu-id="aa776-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa776-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa776-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa776-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa776-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa776-145">Request</span></span>
<span data-ttu-id="aa776-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa776-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aa776-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa776-147">Response</span></span>
<span data-ttu-id="aa776-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa776-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









