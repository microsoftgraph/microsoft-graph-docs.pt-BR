---
title: Atualizar managedEBookAssignment
description: Atualizar as propriedades de um objeto managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bde99a2577fbca953c9b582c238b428d9492b6d0
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44174906"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="0d21e-103">Atualizar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="0d21e-103">Update managedEBookAssignment</span></span>

<span data-ttu-id="0d21e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d21e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d21e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0d21e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d21e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0d21e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d21e-107">Atualizar as propriedades de um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0d21e-107">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d21e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0d21e-108">Prerequisites</span></span>
<span data-ttu-id="0d21e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d21e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d21e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d21e-111">Permission type</span></span>|<span data-ttu-id="0d21e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0d21e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d21e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d21e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d21e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d21e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0d21e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d21e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d21e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d21e-116">Not supported.</span></span>|
|<span data-ttu-id="0d21e-117">Application</span><span class="sxs-lookup"><span data-stu-id="0d21e-117">Application</span></span>|<span data-ttu-id="0d21e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d21e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d21e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d21e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="0d21e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d21e-120">Request headers</span></span>
|<span data-ttu-id="0d21e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0d21e-121">Header</span></span>|<span data-ttu-id="0d21e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0d21e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d21e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d21e-123">Authorization</span></span>|<span data-ttu-id="0d21e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d21e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d21e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0d21e-125">Accept</span></span>|<span data-ttu-id="0d21e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d21e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d21e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d21e-127">Request body</span></span>
<span data-ttu-id="0d21e-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0d21e-128">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="0d21e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0d21e-129">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="0d21e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d21e-130">Property</span></span>|<span data-ttu-id="0d21e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d21e-131">Type</span></span>|<span data-ttu-id="0d21e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d21e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d21e-133">id</span><span class="sxs-lookup"><span data-stu-id="0d21e-133">id</span></span>|<span data-ttu-id="0d21e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d21e-134">String</span></span>|<span data-ttu-id="0d21e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0d21e-135">Key of the entity.</span></span>|
|<span data-ttu-id="0d21e-136">destino</span><span class="sxs-lookup"><span data-stu-id="0d21e-136">target</span></span>|[<span data-ttu-id="0d21e-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0d21e-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0d21e-138">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="0d21e-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="0d21e-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="0d21e-139">installIntent</span></span>|[<span data-ttu-id="0d21e-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="0d21e-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="0d21e-141">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="0d21e-141">The install intent for eBook.</span></span> <span data-ttu-id="0d21e-142">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="0d21e-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="0d21e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d21e-143">Response</span></span>
<span data-ttu-id="0d21e-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d21e-144">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d21e-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d21e-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d21e-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d21e-146">Request</span></span>
<span data-ttu-id="0d21e-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d21e-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 188

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="0d21e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d21e-148">Response</span></span>
<span data-ttu-id="0d21e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d21e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "installIntent": "required"
}
```



