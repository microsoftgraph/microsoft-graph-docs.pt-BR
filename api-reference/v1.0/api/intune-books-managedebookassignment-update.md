---
title: Atualizar managedEBookAssignment
description: Atualizar as propriedades de um objeto managedEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d17b08a32e09a121cf1d9877640c63ad888b045
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261905"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="fcc26-103">Atualizar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="fcc26-103">Update managedEBookAssignment</span></span>

> <span data-ttu-id="fcc26-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fcc26-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcc26-105">Atualizar as propriedades de um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fcc26-105">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcc26-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fcc26-106">Prerequisites</span></span>
<span data-ttu-id="fcc26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fcc26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fcc26-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcc26-109">Permission type</span></span>|<span data-ttu-id="fcc26-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fcc26-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcc26-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcc26-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fcc26-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcc26-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fcc26-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcc26-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcc26-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcc26-114">Not supported.</span></span>|
|<span data-ttu-id="fcc26-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fcc26-115">Application</span></span>|<span data-ttu-id="fcc26-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcc26-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcc26-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcc26-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="fcc26-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fcc26-118">Request headers</span></span>
|<span data-ttu-id="fcc26-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fcc26-119">Header</span></span>|<span data-ttu-id="fcc26-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fcc26-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcc26-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcc26-121">Authorization</span></span>|<span data-ttu-id="fcc26-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcc26-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcc26-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fcc26-123">Accept</span></span>|<span data-ttu-id="fcc26-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fcc26-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcc26-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcc26-125">Request body</span></span>
<span data-ttu-id="fcc26-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fcc26-126">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="fcc26-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fcc26-127">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="fcc26-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fcc26-128">Property</span></span>|<span data-ttu-id="fcc26-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcc26-129">Type</span></span>|<span data-ttu-id="fcc26-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcc26-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcc26-131">id</span><span class="sxs-lookup"><span data-stu-id="fcc26-131">id</span></span>|<span data-ttu-id="fcc26-132">String</span><span class="sxs-lookup"><span data-stu-id="fcc26-132">String</span></span>|<span data-ttu-id="fcc26-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fcc26-133">Key of the entity.</span></span>|
|<span data-ttu-id="fcc26-134">destino</span><span class="sxs-lookup"><span data-stu-id="fcc26-134">target</span></span>|[<span data-ttu-id="fcc26-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fcc26-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fcc26-136">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="fcc26-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="fcc26-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="fcc26-137">installIntent</span></span>|[<span data-ttu-id="fcc26-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="fcc26-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="fcc26-139">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="fcc26-139">The install intent for eBook.</span></span> <span data-ttu-id="fcc26-140">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="fcc26-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="fcc26-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcc26-141">Response</span></span>
<span data-ttu-id="fcc26-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fcc26-142">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcc26-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fcc26-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcc26-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcc26-144">Request</span></span>
<span data-ttu-id="fcc26-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcc26-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fcc26-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcc26-146">Response</span></span>
<span data-ttu-id="fcc26-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fcc26-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



