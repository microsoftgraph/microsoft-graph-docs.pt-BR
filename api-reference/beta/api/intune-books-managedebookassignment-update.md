---
title: Atualizar managedEBookAssignment
description: Atualizar as propriedades de um objeto managedEBookAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14a351ffce07f18e82fefd59bd822523f03b7250
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444571"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="c8130-103">Atualizar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="c8130-103">Update managedEBookAssignment</span></span>

<span data-ttu-id="c8130-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c8130-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8130-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8130-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8130-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8130-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8130-107">Atualizar as propriedades de um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c8130-107">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8130-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8130-108">Prerequisites</span></span>
<span data-ttu-id="c8130-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8130-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8130-111">Permission type</span></span>|<span data-ttu-id="c8130-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c8130-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8130-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8130-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8130-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8130-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c8130-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8130-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8130-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8130-116">Not supported.</span></span>|
|<span data-ttu-id="c8130-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8130-117">Application</span></span>|<span data-ttu-id="c8130-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8130-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8130-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8130-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c8130-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8130-120">Request headers</span></span>
|<span data-ttu-id="c8130-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8130-121">Header</span></span>|<span data-ttu-id="c8130-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c8130-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8130-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8130-123">Authorization</span></span>|<span data-ttu-id="c8130-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8130-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8130-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8130-125">Accept</span></span>|<span data-ttu-id="c8130-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8130-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8130-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8130-127">Request body</span></span>
<span data-ttu-id="c8130-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c8130-128">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="c8130-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c8130-129">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="c8130-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8130-130">Property</span></span>|<span data-ttu-id="c8130-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8130-131">Type</span></span>|<span data-ttu-id="c8130-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8130-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8130-133">id</span><span class="sxs-lookup"><span data-stu-id="c8130-133">id</span></span>|<span data-ttu-id="c8130-134">String</span><span class="sxs-lookup"><span data-stu-id="c8130-134">String</span></span>|<span data-ttu-id="c8130-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c8130-135">Key of the entity.</span></span>|
|<span data-ttu-id="c8130-136">destino</span><span class="sxs-lookup"><span data-stu-id="c8130-136">target</span></span>|[<span data-ttu-id="c8130-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c8130-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c8130-138">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c8130-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="c8130-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="c8130-139">installIntent</span></span>|[<span data-ttu-id="c8130-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="c8130-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="c8130-141">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c8130-141">The install intent for eBook.</span></span> <span data-ttu-id="c8130-142">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="c8130-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="c8130-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8130-143">Response</span></span>
<span data-ttu-id="c8130-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8130-144">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8130-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8130-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8130-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8130-146">Request</span></span>
<span data-ttu-id="c8130-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8130-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c8130-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8130-148">Response</span></span>
<span data-ttu-id="c8130-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8130-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





