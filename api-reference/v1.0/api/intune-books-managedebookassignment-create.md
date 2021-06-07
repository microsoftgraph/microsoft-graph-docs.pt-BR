---
title: Criar managedEBookAssignment
description: Criar um novo objeto managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 881c22ada3a6a4484628a8f5606029cc7f6c4ece
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757259"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="f4647-103">Criar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="f4647-103">Create managedEBookAssignment</span></span>

<span data-ttu-id="f4647-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4647-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4647-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4647-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4647-106">Criar um novo objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f4647-106">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4647-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4647-107">Prerequisites</span></span>
<span data-ttu-id="f4647-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4647-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4647-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4647-110">Permission type</span></span>|<span data-ttu-id="f4647-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4647-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4647-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4647-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4647-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4647-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f4647-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4647-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4647-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4647-115">Not supported.</span></span>|
|<span data-ttu-id="f4647-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4647-116">Application</span></span>|<span data-ttu-id="f4647-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4647-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4647-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4647-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f4647-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4647-119">Request headers</span></span>
|<span data-ttu-id="f4647-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4647-120">Header</span></span>|<span data-ttu-id="f4647-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f4647-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4647-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4647-122">Authorization</span></span>|<span data-ttu-id="f4647-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4647-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4647-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4647-124">Accept</span></span>|<span data-ttu-id="f4647-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4647-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4647-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4647-126">Request body</span></span>
<span data-ttu-id="f4647-127">No corpo da solicitação, forneça uma representação JSON do objeto managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="f4647-127">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="f4647-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="f4647-128">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="f4647-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4647-129">Property</span></span>|<span data-ttu-id="f4647-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4647-130">Type</span></span>|<span data-ttu-id="f4647-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4647-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4647-132">id</span><span class="sxs-lookup"><span data-stu-id="f4647-132">id</span></span>|<span data-ttu-id="f4647-133">String</span><span class="sxs-lookup"><span data-stu-id="f4647-133">String</span></span>|<span data-ttu-id="f4647-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f4647-134">Key of the entity.</span></span>|
|<span data-ttu-id="f4647-135">destino</span><span class="sxs-lookup"><span data-stu-id="f4647-135">target</span></span>|[<span data-ttu-id="f4647-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f4647-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f4647-137">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="f4647-137">The assignment target for eBook.</span></span>|
|<span data-ttu-id="f4647-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="f4647-138">installIntent</span></span>|[<span data-ttu-id="f4647-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="f4647-139">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="f4647-140">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="f4647-140">The install intent for eBook.</span></span> <span data-ttu-id="f4647-141">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="f4647-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="f4647-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4647-142">Response</span></span>
<span data-ttu-id="f4647-143">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4647-143">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4647-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4647-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4647-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4647-145">Request</span></span>
<span data-ttu-id="f4647-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4647-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="f4647-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4647-147">Response</span></span>
<span data-ttu-id="f4647-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4647-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




