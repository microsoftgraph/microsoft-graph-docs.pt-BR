---
title: Criar iosVppEBookAssignment
description: Criar um novo objeto iosVppEBookAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 98508598c74e2038ba61573b3285cd91a2b0c7f2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444557"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="8a1d1-103">Criar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="8a1d1-103">Create iosVppEBookAssignment</span></span>

<span data-ttu-id="8a1d1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8a1d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a1d1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8a1d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a1d1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8a1d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a1d1-107">Criar um novo objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8a1d1-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a1d1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a1d1-108">Prerequisites</span></span>
<span data-ttu-id="8a1d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a1d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a1d1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a1d1-111">Permission type</span></span>|<span data-ttu-id="8a1d1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8a1d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a1d1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a1d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a1d1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a1d1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8a1d1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a1d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a1d1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a1d1-116">Not supported.</span></span>|
|<span data-ttu-id="8a1d1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a1d1-117">Application</span></span>|<span data-ttu-id="8a1d1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a1d1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a1d1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a1d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8a1d1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a1d1-120">Request headers</span></span>
|<span data-ttu-id="8a1d1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a1d1-121">Header</span></span>|<span data-ttu-id="8a1d1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8a1d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a1d1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a1d1-123">Authorization</span></span>|<span data-ttu-id="8a1d1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a1d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a1d1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8a1d1-125">Accept</span></span>|<span data-ttu-id="8a1d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a1d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a1d1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a1d1-127">Request body</span></span>
<span data-ttu-id="8a1d1-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="8a1d1-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="8a1d1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="8a1d1-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="8a1d1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a1d1-130">Property</span></span>|<span data-ttu-id="8a1d1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a1d1-131">Type</span></span>|<span data-ttu-id="8a1d1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a1d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a1d1-133">id</span><span class="sxs-lookup"><span data-stu-id="8a1d1-133">id</span></span>|<span data-ttu-id="8a1d1-134">String</span><span class="sxs-lookup"><span data-stu-id="8a1d1-134">String</span></span>|<span data-ttu-id="8a1d1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8a1d1-135">Key of the entity.</span></span> <span data-ttu-id="8a1d1-136">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8a1d1-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="8a1d1-137">destino</span><span class="sxs-lookup"><span data-stu-id="8a1d1-137">target</span></span>|[<span data-ttu-id="8a1d1-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8a1d1-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8a1d1-139">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="8a1d1-139">The assignment target for eBook.</span></span> <span data-ttu-id="8a1d1-140">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8a1d1-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="8a1d1-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="8a1d1-141">installIntent</span></span>|[<span data-ttu-id="8a1d1-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="8a1d1-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="8a1d1-143">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="8a1d1-143">The install intent for eBook.</span></span> <span data-ttu-id="8a1d1-144">Herdado de [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8a1d1-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="8a1d1-145">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="8a1d1-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="8a1d1-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a1d1-146">Response</span></span>
<span data-ttu-id="8a1d1-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a1d1-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a1d1-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a1d1-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a1d1-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a1d1-149">Request</span></span>
<span data-ttu-id="8a1d1-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a1d1-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="8a1d1-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a1d1-151">Response</span></span>
<span data-ttu-id="8a1d1-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a1d1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





