---
title: Atualizar iosVppEBookAssignment
description: Atualizar as propriedades de um objeto iosVppEBookAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ced3d7e40427c7d6b93873f3fb9cfa7fa4060f4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972302"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="80fa6-103">Atualizar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="80fa6-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="80fa6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="80fa6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80fa6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80fa6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80fa6-106">Atualizar as propriedades de um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="80fa6-106">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80fa6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80fa6-107">Prerequisites</span></span>
<span data-ttu-id="80fa6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80fa6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80fa6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80fa6-110">Permission type</span></span>|<span data-ttu-id="80fa6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="80fa6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80fa6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80fa6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80fa6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80fa6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="80fa6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80fa6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80fa6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80fa6-115">Not supported.</span></span>|
|<span data-ttu-id="80fa6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80fa6-116">Application</span></span>|<span data-ttu-id="80fa6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80fa6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80fa6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80fa6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="80fa6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80fa6-119">Request headers</span></span>
|<span data-ttu-id="80fa6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80fa6-120">Header</span></span>|<span data-ttu-id="80fa6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="80fa6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80fa6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="80fa6-122">Authorization</span></span>|<span data-ttu-id="80fa6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80fa6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80fa6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="80fa6-124">Accept</span></span>|<span data-ttu-id="80fa6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80fa6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80fa6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80fa6-126">Request body</span></span>
<span data-ttu-id="80fa6-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="80fa6-127">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="80fa6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="80fa6-128">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="80fa6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80fa6-129">Property</span></span>|<span data-ttu-id="80fa6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="80fa6-130">Type</span></span>|<span data-ttu-id="80fa6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="80fa6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80fa6-132">id</span><span class="sxs-lookup"><span data-stu-id="80fa6-132">id</span></span>|<span data-ttu-id="80fa6-133">String</span><span class="sxs-lookup"><span data-stu-id="80fa6-133">String</span></span>|<span data-ttu-id="80fa6-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="80fa6-134">Key of the entity.</span></span> <span data-ttu-id="80fa6-135">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="80fa6-135">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="80fa6-136">destino</span><span class="sxs-lookup"><span data-stu-id="80fa6-136">target</span></span>|[<span data-ttu-id="80fa6-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="80fa6-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="80fa6-138">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="80fa6-138">The assignment target for eBook.</span></span> <span data-ttu-id="80fa6-139">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="80fa6-139">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="80fa6-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="80fa6-140">installIntent</span></span>|[<span data-ttu-id="80fa6-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="80fa6-141">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="80fa6-142">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="80fa6-142">The install intent for eBook.</span></span> <span data-ttu-id="80fa6-143">Herdado de [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="80fa6-143">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="80fa6-144">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="80fa6-144">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="80fa6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="80fa6-145">Response</span></span>
<span data-ttu-id="80fa6-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80fa6-146">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80fa6-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80fa6-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="80fa6-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80fa6-148">Request</span></span>
<span data-ttu-id="80fa6-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80fa6-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80fa6-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="80fa6-150">Response</span></span>
<span data-ttu-id="80fa6-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80fa6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





