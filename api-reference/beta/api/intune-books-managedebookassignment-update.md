---
title: Atualizar managedEBookAssignment
description: Atualizar as propriedades de um objeto managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d1adfc73c4986605a1a70ed2b5f3ca0dfcf1fd5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133070"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="b6fdf-103">Atualizar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="b6fdf-103">Update managedEBookAssignment</span></span>

<span data-ttu-id="b6fdf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6fdf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6fdf-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6fdf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6fdf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6fdf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6fdf-107">Atualizar as propriedades de um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b6fdf-107">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6fdf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6fdf-108">Prerequisites</span></span>
<span data-ttu-id="b6fdf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6fdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6fdf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6fdf-111">Permission type</span></span>|<span data-ttu-id="b6fdf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6fdf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6fdf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6fdf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6fdf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6fdf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b6fdf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6fdf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6fdf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6fdf-116">Not supported.</span></span>|
|<span data-ttu-id="b6fdf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6fdf-117">Application</span></span>|<span data-ttu-id="b6fdf-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6fdf-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6fdf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6fdf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b6fdf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6fdf-120">Request headers</span></span>
|<span data-ttu-id="b6fdf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6fdf-121">Header</span></span>|<span data-ttu-id="b6fdf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6fdf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6fdf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6fdf-123">Authorization</span></span>|<span data-ttu-id="b6fdf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6fdf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6fdf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6fdf-125">Accept</span></span>|<span data-ttu-id="b6fdf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6fdf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6fdf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6fdf-127">Request body</span></span>
<span data-ttu-id="b6fdf-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b6fdf-128">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="b6fdf-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b6fdf-129">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="b6fdf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6fdf-130">Property</span></span>|<span data-ttu-id="b6fdf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6fdf-131">Type</span></span>|<span data-ttu-id="b6fdf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6fdf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6fdf-133">id</span><span class="sxs-lookup"><span data-stu-id="b6fdf-133">id</span></span>|<span data-ttu-id="b6fdf-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6fdf-134">String</span></span>|<span data-ttu-id="b6fdf-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b6fdf-135">Key of the entity.</span></span>|
|<span data-ttu-id="b6fdf-136">destino</span><span class="sxs-lookup"><span data-stu-id="b6fdf-136">target</span></span>|[<span data-ttu-id="b6fdf-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b6fdf-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b6fdf-138">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="b6fdf-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="b6fdf-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="b6fdf-139">installIntent</span></span>|[<span data-ttu-id="b6fdf-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="b6fdf-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="b6fdf-141">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="b6fdf-141">The install intent for eBook.</span></span> <span data-ttu-id="b6fdf-142">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="b6fdf-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="b6fdf-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6fdf-143">Response</span></span>
<span data-ttu-id="b6fdf-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6fdf-144">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6fdf-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6fdf-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6fdf-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6fdf-146">Request</span></span>
<span data-ttu-id="b6fdf-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6fdf-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6fdf-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6fdf-148">Response</span></span>
<span data-ttu-id="b6fdf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6fdf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




