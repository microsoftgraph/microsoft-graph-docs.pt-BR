---
title: Criar iosVppEBookAssignment
description: Criar um novo objeto iosVppEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f6aa4201d5801f3e235fa28a44d0e38f69fd1bd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133189"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="17f03-103">Criar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="17f03-103">Create iosVppEBookAssignment</span></span>

<span data-ttu-id="17f03-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17f03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17f03-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="17f03-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17f03-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17f03-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17f03-107">Criar um novo objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="17f03-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17f03-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17f03-108">Prerequisites</span></span>
<span data-ttu-id="17f03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17f03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17f03-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17f03-111">Permission type</span></span>|<span data-ttu-id="17f03-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17f03-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17f03-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17f03-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17f03-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17f03-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="17f03-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17f03-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17f03-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17f03-116">Not supported.</span></span>|
|<span data-ttu-id="17f03-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17f03-117">Application</span></span>|<span data-ttu-id="17f03-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17f03-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17f03-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17f03-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="17f03-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17f03-120">Request headers</span></span>
|<span data-ttu-id="17f03-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17f03-121">Header</span></span>|<span data-ttu-id="17f03-122">Valor</span><span class="sxs-lookup"><span data-stu-id="17f03-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17f03-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="17f03-123">Authorization</span></span>|<span data-ttu-id="17f03-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17f03-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17f03-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17f03-125">Accept</span></span>|<span data-ttu-id="17f03-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17f03-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17f03-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17f03-127">Request body</span></span>
<span data-ttu-id="17f03-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="17f03-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="17f03-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="17f03-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="17f03-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17f03-130">Property</span></span>|<span data-ttu-id="17f03-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="17f03-131">Type</span></span>|<span data-ttu-id="17f03-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="17f03-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17f03-133">id</span><span class="sxs-lookup"><span data-stu-id="17f03-133">id</span></span>|<span data-ttu-id="17f03-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17f03-134">String</span></span>|<span data-ttu-id="17f03-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="17f03-135">Key of the entity.</span></span> <span data-ttu-id="17f03-136">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="17f03-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="17f03-137">destino</span><span class="sxs-lookup"><span data-stu-id="17f03-137">target</span></span>|[<span data-ttu-id="17f03-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="17f03-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="17f03-139">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="17f03-139">The assignment target for eBook.</span></span> <span data-ttu-id="17f03-140">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="17f03-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="17f03-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="17f03-141">installIntent</span></span>|[<span data-ttu-id="17f03-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="17f03-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="17f03-143">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="17f03-143">The install intent for eBook.</span></span> <span data-ttu-id="17f03-144">Herdado [de managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="17f03-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="17f03-145">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="17f03-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="17f03-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="17f03-146">Response</span></span>
<span data-ttu-id="17f03-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17f03-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17f03-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17f03-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="17f03-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17f03-149">Request</span></span>
<span data-ttu-id="17f03-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17f03-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="17f03-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="17f03-151">Response</span></span>
<span data-ttu-id="17f03-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17f03-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "48f05789-5789-48f0-8957-f0488957f048",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "installIntent": "required"
}
```




