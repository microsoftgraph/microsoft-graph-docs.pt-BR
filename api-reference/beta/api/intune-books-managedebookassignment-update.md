---
title: Atualizar managedEBookAssignment
description: Atualizar as propriedades de um objeto managedEBookAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 708a7aa3266e67d62ce540c3f5e2f22b8154912b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335939"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="ae156-103">Atualizar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="ae156-103">Update managedEBookAssignment</span></span>

> <span data-ttu-id="ae156-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae156-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae156-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae156-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae156-106">Atualizar as propriedades de um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ae156-106">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae156-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae156-107">Prerequisites</span></span>
<span data-ttu-id="ae156-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae156-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae156-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae156-110">Permission type</span></span>|<span data-ttu-id="ae156-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae156-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae156-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae156-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae156-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae156-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ae156-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae156-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae156-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae156-115">Not supported.</span></span>|
|<span data-ttu-id="ae156-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae156-116">Application</span></span>|<span data-ttu-id="ae156-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae156-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae156-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae156-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ae156-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae156-119">Request headers</span></span>
|<span data-ttu-id="ae156-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae156-120">Header</span></span>|<span data-ttu-id="ae156-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ae156-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae156-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae156-122">Authorization</span></span>|<span data-ttu-id="ae156-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae156-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae156-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae156-124">Accept</span></span>|<span data-ttu-id="ae156-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae156-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae156-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae156-126">Request body</span></span>
<span data-ttu-id="ae156-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ae156-127">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="ae156-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ae156-128">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="ae156-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae156-129">Property</span></span>|<span data-ttu-id="ae156-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae156-130">Type</span></span>|<span data-ttu-id="ae156-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae156-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae156-132">id</span><span class="sxs-lookup"><span data-stu-id="ae156-132">id</span></span>|<span data-ttu-id="ae156-133">String</span><span class="sxs-lookup"><span data-stu-id="ae156-133">String</span></span>|<span data-ttu-id="ae156-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ae156-134">Key of the entity.</span></span>|
|<span data-ttu-id="ae156-135">destino</span><span class="sxs-lookup"><span data-stu-id="ae156-135">target</span></span>|[<span data-ttu-id="ae156-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ae156-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ae156-137">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="ae156-137">The assignment target for eBook.</span></span>|
|<span data-ttu-id="ae156-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="ae156-138">installIntent</span></span>|[<span data-ttu-id="ae156-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="ae156-139">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="ae156-140">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="ae156-140">The install intent for eBook.</span></span> <span data-ttu-id="ae156-141">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="ae156-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="ae156-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae156-142">Response</span></span>
<span data-ttu-id="ae156-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae156-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae156-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae156-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae156-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae156-145">Request</span></span>
<span data-ttu-id="ae156-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae156-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="ae156-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae156-147">Response</span></span>
<span data-ttu-id="ae156-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae156-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






