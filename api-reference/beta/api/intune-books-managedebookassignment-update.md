---
title: Atualizar managedEBookAssignment
description: Atualizar as propriedades de um objeto managedEBookAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0cf6aef49315eba7f6c67af34147a577a43a5a80
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413791"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="ff5d6-103">Atualizar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="ff5d6-103">Update managedEBookAssignment</span></span>

> <span data-ttu-id="ff5d6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ff5d6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ff5d6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ff5d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff5d6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ff5d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff5d6-107">Atualizar as propriedades de um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff5d6-107">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff5d6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff5d6-108">Prerequisites</span></span>
<span data-ttu-id="ff5d6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ff5d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ff5d6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff5d6-111">Permission type</span></span>|<span data-ttu-id="ff5d6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff5d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff5d6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff5d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff5d6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff5d6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ff5d6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff5d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff5d6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff5d6-116">Not supported.</span></span>|
|<span data-ttu-id="ff5d6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff5d6-117">Application</span></span>|<span data-ttu-id="ff5d6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff5d6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff5d6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff5d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ff5d6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff5d6-120">Request headers</span></span>
|<span data-ttu-id="ff5d6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff5d6-121">Header</span></span>|<span data-ttu-id="ff5d6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ff5d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff5d6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff5d6-123">Authorization</span></span>|<span data-ttu-id="ff5d6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff5d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff5d6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff5d6-125">Accept</span></span>|<span data-ttu-id="ff5d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff5d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff5d6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff5d6-127">Request body</span></span>
<span data-ttu-id="ff5d6-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff5d6-128">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="ff5d6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff5d6-129">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="ff5d6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff5d6-130">Property</span></span>|<span data-ttu-id="ff5d6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff5d6-131">Type</span></span>|<span data-ttu-id="ff5d6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff5d6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff5d6-133">id</span><span class="sxs-lookup"><span data-stu-id="ff5d6-133">id</span></span>|<span data-ttu-id="ff5d6-134">String</span><span class="sxs-lookup"><span data-stu-id="ff5d6-134">String</span></span>|<span data-ttu-id="ff5d6-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ff5d6-135">Key of the entity.</span></span>|
|<span data-ttu-id="ff5d6-136">destino</span><span class="sxs-lookup"><span data-stu-id="ff5d6-136">target</span></span>|[<span data-ttu-id="ff5d6-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ff5d6-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ff5d6-138">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="ff5d6-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="ff5d6-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="ff5d6-139">installIntent</span></span>|[<span data-ttu-id="ff5d6-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="ff5d6-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="ff5d6-141">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="ff5d6-141">The install intent for eBook.</span></span> <span data-ttu-id="ff5d6-142">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="ff5d6-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="ff5d6-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff5d6-143">Response</span></span>
<span data-ttu-id="ff5d6-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff5d6-144">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff5d6-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff5d6-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff5d6-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff5d6-146">Request</span></span>
<span data-ttu-id="ff5d6-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff5d6-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ff5d6-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff5d6-148">Response</span></span>
<span data-ttu-id="ff5d6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff5d6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




