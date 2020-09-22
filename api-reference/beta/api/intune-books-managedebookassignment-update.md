---
title: Atualizar managedEBookAssignment
description: Atualizar as propriedades de um objeto managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 77bec02071b2f3e43cefd560b05873ed59f0eb60
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975511"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="04845-103">Atualizar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="04845-103">Update managedEBookAssignment</span></span>

<span data-ttu-id="04845-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04845-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04845-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04845-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04845-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04845-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04845-107">Atualizar as propriedades de um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="04845-107">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04845-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04845-108">Prerequisites</span></span>
<span data-ttu-id="04845-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04845-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04845-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04845-111">Permission type</span></span>|<span data-ttu-id="04845-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="04845-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04845-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04845-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04845-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04845-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04845-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04845-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04845-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04845-116">Not supported.</span></span>|
|<span data-ttu-id="04845-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04845-117">Application</span></span>|<span data-ttu-id="04845-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04845-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04845-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04845-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="04845-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04845-120">Request headers</span></span>
|<span data-ttu-id="04845-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04845-121">Header</span></span>|<span data-ttu-id="04845-122">Valor</span><span class="sxs-lookup"><span data-stu-id="04845-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04845-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="04845-123">Authorization</span></span>|<span data-ttu-id="04845-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04845-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04845-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04845-125">Accept</span></span>|<span data-ttu-id="04845-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04845-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04845-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04845-127">Request body</span></span>
<span data-ttu-id="04845-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="04845-128">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="04845-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="04845-129">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="04845-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04845-130">Property</span></span>|<span data-ttu-id="04845-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="04845-131">Type</span></span>|<span data-ttu-id="04845-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="04845-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04845-133">id</span><span class="sxs-lookup"><span data-stu-id="04845-133">id</span></span>|<span data-ttu-id="04845-134">String</span><span class="sxs-lookup"><span data-stu-id="04845-134">String</span></span>|<span data-ttu-id="04845-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="04845-135">Key of the entity.</span></span>|
|<span data-ttu-id="04845-136">destino</span><span class="sxs-lookup"><span data-stu-id="04845-136">target</span></span>|[<span data-ttu-id="04845-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="04845-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="04845-138">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="04845-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="04845-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="04845-139">installIntent</span></span>|[<span data-ttu-id="04845-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="04845-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="04845-141">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="04845-141">The install intent for eBook.</span></span> <span data-ttu-id="04845-142">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="04845-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="04845-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="04845-143">Response</span></span>
<span data-ttu-id="04845-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04845-144">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04845-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04845-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="04845-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04845-146">Request</span></span>
<span data-ttu-id="04845-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04845-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 355

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="04845-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="04845-148">Response</span></span>
<span data-ttu-id="04845-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04845-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 404

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "installIntent": "required"
}
```






