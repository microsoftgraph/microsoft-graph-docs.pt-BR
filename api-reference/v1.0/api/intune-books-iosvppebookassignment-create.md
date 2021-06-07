---
title: Criar iosVppEBookAssignment
description: Criar um novo objeto iosVppEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 38014d5ad851f44555dd637f62ae4923c12ee4bb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758438"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="8335f-103">Criar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="8335f-103">Create iosVppEBookAssignment</span></span>

<span data-ttu-id="8335f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8335f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8335f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8335f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8335f-106">Criar um novo objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8335f-106">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8335f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8335f-107">Prerequisites</span></span>
<span data-ttu-id="8335f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8335f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8335f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8335f-110">Permission type</span></span>|<span data-ttu-id="8335f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8335f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8335f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8335f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8335f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8335f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8335f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8335f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8335f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8335f-115">Not supported.</span></span>|
|<span data-ttu-id="8335f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8335f-116">Application</span></span>|<span data-ttu-id="8335f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8335f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8335f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8335f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8335f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8335f-119">Request headers</span></span>
|<span data-ttu-id="8335f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8335f-120">Header</span></span>|<span data-ttu-id="8335f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8335f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8335f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8335f-122">Authorization</span></span>|<span data-ttu-id="8335f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8335f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8335f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8335f-124">Accept</span></span>|<span data-ttu-id="8335f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8335f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8335f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8335f-126">Request body</span></span>
<span data-ttu-id="8335f-127">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="8335f-127">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="8335f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="8335f-128">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="8335f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8335f-129">Property</span></span>|<span data-ttu-id="8335f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8335f-130">Type</span></span>|<span data-ttu-id="8335f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8335f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8335f-132">id</span><span class="sxs-lookup"><span data-stu-id="8335f-132">id</span></span>|<span data-ttu-id="8335f-133">String</span><span class="sxs-lookup"><span data-stu-id="8335f-133">String</span></span>|<span data-ttu-id="8335f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8335f-134">Key of the entity.</span></span> <span data-ttu-id="8335f-135">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8335f-135">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="8335f-136">destino</span><span class="sxs-lookup"><span data-stu-id="8335f-136">target</span></span>|[<span data-ttu-id="8335f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8335f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8335f-138">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="8335f-138">The assignment target for eBook.</span></span> <span data-ttu-id="8335f-139">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8335f-139">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="8335f-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="8335f-140">installIntent</span></span>|[<span data-ttu-id="8335f-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="8335f-141">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="8335f-142">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="8335f-142">The install intent for eBook.</span></span> <span data-ttu-id="8335f-143">Herdado [de managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8335f-143">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="8335f-144">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="8335f-144">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="8335f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8335f-145">Response</span></span>
<span data-ttu-id="8335f-146">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8335f-146">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8335f-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8335f-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="8335f-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8335f-148">Request</span></span>
<span data-ttu-id="8335f-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8335f-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8335f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="8335f-150">Response</span></span>
<span data-ttu-id="8335f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8335f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




