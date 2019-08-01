---
title: Atualizar managedEBookAssignment
description: Atualizar as propriedades de um objeto managedEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1e4f7d8fe21e05517d6fdd4738f2e1a2f24b5d36
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019965"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="68179-103">Atualizar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="68179-103">Update managedEBookAssignment</span></span>

> <span data-ttu-id="68179-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="68179-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68179-105">Atualizar as propriedades de um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="68179-105">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68179-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="68179-106">Prerequisites</span></span>
<span data-ttu-id="68179-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68179-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68179-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68179-109">Permission type</span></span>|<span data-ttu-id="68179-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="68179-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68179-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68179-111">Delegated (work or school account)</span></span>|<span data-ttu-id="68179-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68179-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="68179-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68179-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68179-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68179-114">Not supported.</span></span>|
|<span data-ttu-id="68179-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68179-115">Application</span></span>|<span data-ttu-id="68179-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68179-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68179-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68179-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="68179-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68179-118">Request headers</span></span>
|<span data-ttu-id="68179-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="68179-119">Header</span></span>|<span data-ttu-id="68179-120">Valor</span><span class="sxs-lookup"><span data-stu-id="68179-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68179-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="68179-121">Authorization</span></span>|<span data-ttu-id="68179-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68179-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68179-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="68179-123">Accept</span></span>|<span data-ttu-id="68179-124">application/json</span><span class="sxs-lookup"><span data-stu-id="68179-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68179-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68179-125">Request body</span></span>
<span data-ttu-id="68179-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="68179-126">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="68179-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="68179-127">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="68179-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68179-128">Property</span></span>|<span data-ttu-id="68179-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="68179-129">Type</span></span>|<span data-ttu-id="68179-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="68179-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68179-131">id</span><span class="sxs-lookup"><span data-stu-id="68179-131">id</span></span>|<span data-ttu-id="68179-132">String</span><span class="sxs-lookup"><span data-stu-id="68179-132">String</span></span>|<span data-ttu-id="68179-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="68179-133">Key of the entity.</span></span>|
|<span data-ttu-id="68179-134">destino</span><span class="sxs-lookup"><span data-stu-id="68179-134">target</span></span>|[<span data-ttu-id="68179-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="68179-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="68179-136">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="68179-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="68179-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="68179-137">installIntent</span></span>|[<span data-ttu-id="68179-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="68179-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="68179-139">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="68179-139">The install intent for eBook.</span></span> <span data-ttu-id="68179-140">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="68179-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="68179-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="68179-141">Response</span></span>
<span data-ttu-id="68179-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68179-142">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68179-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68179-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="68179-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68179-144">Request</span></span>
<span data-ttu-id="68179-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68179-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="68179-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="68179-146">Response</span></span>
<span data-ttu-id="68179-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68179-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



