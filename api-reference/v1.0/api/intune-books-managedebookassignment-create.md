---
title: Criar managedEBookAssignment
description: Criar um novo objeto managedEBookAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c30894d22f1e901046d30f3605317c2bde890fc
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357882"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="e59d2-103">Criar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="e59d2-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="e59d2-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e59d2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e59d2-105">Criar um novo objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e59d2-105">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e59d2-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e59d2-106">Prerequisites</span></span>
<span data-ttu-id="e59d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e59d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e59d2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e59d2-109">Permission type</span></span>|<span data-ttu-id="e59d2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e59d2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e59d2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e59d2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e59d2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e59d2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e59d2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e59d2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e59d2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e59d2-114">Not supported.</span></span>|
|<span data-ttu-id="e59d2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e59d2-115">Application</span></span>|<span data-ttu-id="e59d2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e59d2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e59d2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e59d2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e59d2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e59d2-118">Request headers</span></span>
|<span data-ttu-id="e59d2-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e59d2-119">Header</span></span>|<span data-ttu-id="e59d2-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e59d2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e59d2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e59d2-121">Authorization</span></span>|<span data-ttu-id="e59d2-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e59d2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e59d2-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e59d2-123">Accept</span></span>|<span data-ttu-id="e59d2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e59d2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e59d2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e59d2-125">Request body</span></span>
<span data-ttu-id="e59d2-126">No corpo da solicitação, forneça uma representação JSON do objeto managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="e59d2-126">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="e59d2-127">A tabela a seguir mostra as propriedades que são necessárias ao criar managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="e59d2-127">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="e59d2-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e59d2-128">Property</span></span>|<span data-ttu-id="e59d2-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e59d2-129">Type</span></span>|<span data-ttu-id="e59d2-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e59d2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e59d2-131">id</span><span class="sxs-lookup"><span data-stu-id="e59d2-131">id</span></span>|<span data-ttu-id="e59d2-132">String</span><span class="sxs-lookup"><span data-stu-id="e59d2-132">String</span></span>|<span data-ttu-id="e59d2-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e59d2-133">Key of the entity.</span></span>|
|<span data-ttu-id="e59d2-134">destino</span><span class="sxs-lookup"><span data-stu-id="e59d2-134">target</span></span>|[<span data-ttu-id="e59d2-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e59d2-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e59d2-136">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="e59d2-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="e59d2-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="e59d2-137">installIntent</span></span>|[<span data-ttu-id="e59d2-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="e59d2-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="e59d2-139">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="e59d2-139">The install intent for eBook.</span></span> <span data-ttu-id="e59d2-140">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="e59d2-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="e59d2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e59d2-141">Response</span></span>
<span data-ttu-id="e59d2-142">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e59d2-142">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e59d2-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e59d2-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="e59d2-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e59d2-144">Request</span></span>
<span data-ttu-id="e59d2-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e59d2-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e59d2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e59d2-146">Response</span></span>
<span data-ttu-id="e59d2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e59d2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




