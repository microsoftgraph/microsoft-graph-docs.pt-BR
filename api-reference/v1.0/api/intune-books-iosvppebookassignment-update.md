---
title: Atualizar iosVppEBookAssignment
description: Atualizar as propriedades de um objeto iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1af37aaf787c7909d1d3653d196ebb19b68476cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524960"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="15970-103">Atualizar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="15970-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="15970-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15970-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15970-105">Atualizar as propriedades de um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="15970-105">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15970-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15970-106">Prerequisites</span></span>
<span data-ttu-id="15970-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15970-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15970-109">Permission type</span></span>|<span data-ttu-id="15970-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15970-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15970-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15970-111">Delegated (work or school account)</span></span>|<span data-ttu-id="15970-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15970-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="15970-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15970-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15970-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15970-114">Not supported.</span></span>|
|<span data-ttu-id="15970-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15970-115">Application</span></span>|<span data-ttu-id="15970-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15970-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15970-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15970-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="15970-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15970-118">Request headers</span></span>
|<span data-ttu-id="15970-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15970-119">Header</span></span>|<span data-ttu-id="15970-120">Valor</span><span class="sxs-lookup"><span data-stu-id="15970-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15970-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="15970-121">Authorization</span></span>|<span data-ttu-id="15970-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15970-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15970-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15970-123">Accept</span></span>|<span data-ttu-id="15970-124">application/json</span><span class="sxs-lookup"><span data-stu-id="15970-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15970-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15970-125">Request body</span></span>
<span data-ttu-id="15970-126">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="15970-126">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="15970-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="15970-127">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="15970-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15970-128">Property</span></span>|<span data-ttu-id="15970-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="15970-129">Type</span></span>|<span data-ttu-id="15970-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="15970-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15970-131">id</span><span class="sxs-lookup"><span data-stu-id="15970-131">id</span></span>|<span data-ttu-id="15970-132">String</span><span class="sxs-lookup"><span data-stu-id="15970-132">String</span></span>|<span data-ttu-id="15970-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="15970-133">Key of the entity.</span></span> <span data-ttu-id="15970-134">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="15970-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="15970-135">destino</span><span class="sxs-lookup"><span data-stu-id="15970-135">target</span></span>|[<span data-ttu-id="15970-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="15970-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="15970-137">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="15970-137">The assignment target for eBook.</span></span> <span data-ttu-id="15970-138">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="15970-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="15970-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="15970-139">installIntent</span></span>|[<span data-ttu-id="15970-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="15970-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="15970-141">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="15970-141">The install intent for eBook.</span></span> <span data-ttu-id="15970-142">Herdado de [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="15970-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="15970-143">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="15970-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="15970-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="15970-144">Response</span></span>
<span data-ttu-id="15970-145">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15970-145">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15970-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15970-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="15970-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15970-147">Request</span></span>
<span data-ttu-id="15970-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15970-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="15970-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="15970-149">Response</span></span>
<span data-ttu-id="15970-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15970-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



