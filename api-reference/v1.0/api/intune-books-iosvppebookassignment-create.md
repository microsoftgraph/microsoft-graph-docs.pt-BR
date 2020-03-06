---
title: Criar iosVppEBookAssignment
description: Criar um novo objeto iosVppEBookAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0fdd070e495dca9af77f484542405a45e50fe652
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515627"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="73e07-103">Criar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="73e07-103">Create iosVppEBookAssignment</span></span>

<span data-ttu-id="73e07-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73e07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73e07-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73e07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73e07-106">Criar um novo objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="73e07-106">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73e07-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73e07-107">Prerequisites</span></span>
<span data-ttu-id="73e07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73e07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73e07-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73e07-110">Permission type</span></span>|<span data-ttu-id="73e07-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73e07-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73e07-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73e07-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73e07-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73e07-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="73e07-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73e07-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73e07-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73e07-115">Not supported.</span></span>|
|<span data-ttu-id="73e07-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73e07-116">Application</span></span>|<span data-ttu-id="73e07-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73e07-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73e07-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73e07-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="73e07-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73e07-119">Request headers</span></span>
|<span data-ttu-id="73e07-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73e07-120">Header</span></span>|<span data-ttu-id="73e07-121">Valor</span><span class="sxs-lookup"><span data-stu-id="73e07-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73e07-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="73e07-122">Authorization</span></span>|<span data-ttu-id="73e07-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73e07-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73e07-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73e07-124">Accept</span></span>|<span data-ttu-id="73e07-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73e07-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73e07-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73e07-126">Request body</span></span>
<span data-ttu-id="73e07-127">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="73e07-127">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="73e07-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="73e07-128">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="73e07-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73e07-129">Property</span></span>|<span data-ttu-id="73e07-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="73e07-130">Type</span></span>|<span data-ttu-id="73e07-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="73e07-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73e07-132">id</span><span class="sxs-lookup"><span data-stu-id="73e07-132">id</span></span>|<span data-ttu-id="73e07-133">String</span><span class="sxs-lookup"><span data-stu-id="73e07-133">String</span></span>|<span data-ttu-id="73e07-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="73e07-134">Key of the entity.</span></span> <span data-ttu-id="73e07-135">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="73e07-135">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="73e07-136">destino</span><span class="sxs-lookup"><span data-stu-id="73e07-136">target</span></span>|[<span data-ttu-id="73e07-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="73e07-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="73e07-138">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="73e07-138">The assignment target for eBook.</span></span> <span data-ttu-id="73e07-139">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="73e07-139">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="73e07-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="73e07-140">installIntent</span></span>|[<span data-ttu-id="73e07-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="73e07-141">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="73e07-142">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="73e07-142">The install intent for eBook.</span></span> <span data-ttu-id="73e07-143">Herdado de [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="73e07-143">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="73e07-144">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="73e07-144">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="73e07-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="73e07-145">Response</span></span>
<span data-ttu-id="73e07-146">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73e07-146">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73e07-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73e07-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="73e07-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73e07-148">Request</span></span>
<span data-ttu-id="73e07-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73e07-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="73e07-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="73e07-150">Response</span></span>
<span data-ttu-id="73e07-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73e07-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




