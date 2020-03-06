---
title: Criar managedEBookAssignment
description: Criar um novo objeto managedEBookAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 70c5a2c0bfb09214745918be07f2a4ff04f26c78
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515571"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="e2c0c-103">Criar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="e2c0c-103">Create managedEBookAssignment</span></span>

<span data-ttu-id="e2c0c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2c0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2c0c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2c0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2c0c-106">Criar um novo objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e2c0c-106">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2c0c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e2c0c-107">Prerequisites</span></span>
<span data-ttu-id="e2c0c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2c0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2c0c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2c0c-110">Permission type</span></span>|<span data-ttu-id="e2c0c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e2c0c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2c0c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2c0c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2c0c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2c0c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e2c0c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2c0c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2c0c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2c0c-115">Not supported.</span></span>|
|<span data-ttu-id="e2c0c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2c0c-116">Application</span></span>|<span data-ttu-id="e2c0c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2c0c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2c0c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2c0c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e2c0c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2c0c-119">Request headers</span></span>
|<span data-ttu-id="e2c0c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e2c0c-120">Header</span></span>|<span data-ttu-id="e2c0c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e2c0c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2c0c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2c0c-122">Authorization</span></span>|<span data-ttu-id="e2c0c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2c0c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2c0c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e2c0c-124">Accept</span></span>|<span data-ttu-id="e2c0c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e2c0c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2c0c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2c0c-126">Request body</span></span>
<span data-ttu-id="e2c0c-127">No corpo da solicitação, forneça uma representação JSON do objeto managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="e2c0c-127">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="e2c0c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="e2c0c-128">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="e2c0c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2c0c-129">Property</span></span>|<span data-ttu-id="e2c0c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2c0c-130">Type</span></span>|<span data-ttu-id="e2c0c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2c0c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2c0c-132">id</span><span class="sxs-lookup"><span data-stu-id="e2c0c-132">id</span></span>|<span data-ttu-id="e2c0c-133">String</span><span class="sxs-lookup"><span data-stu-id="e2c0c-133">String</span></span>|<span data-ttu-id="e2c0c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e2c0c-134">Key of the entity.</span></span>|
|<span data-ttu-id="e2c0c-135">destino</span><span class="sxs-lookup"><span data-stu-id="e2c0c-135">target</span></span>|[<span data-ttu-id="e2c0c-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e2c0c-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e2c0c-137">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="e2c0c-137">The assignment target for eBook.</span></span>|
|<span data-ttu-id="e2c0c-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="e2c0c-138">installIntent</span></span>|[<span data-ttu-id="e2c0c-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="e2c0c-139">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="e2c0c-140">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="e2c0c-140">The install intent for eBook.</span></span> <span data-ttu-id="e2c0c-141">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="e2c0c-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="e2c0c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2c0c-142">Response</span></span>
<span data-ttu-id="e2c0c-143">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2c0c-143">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2c0c-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2c0c-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2c0c-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2c0c-145">Request</span></span>
<span data-ttu-id="e2c0c-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2c0c-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="e2c0c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2c0c-147">Response</span></span>
<span data-ttu-id="e2c0c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2c0c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




