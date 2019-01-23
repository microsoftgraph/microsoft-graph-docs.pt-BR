---
title: Criar iosVppEBookAssignment
description: Criar um novo objeto iosVppEBookAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3cfebd4f1b61ae7cfc3c4a92d2c3415ce18e4cab
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424501"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="021b9-103">Criar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="021b9-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="021b9-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="021b9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="021b9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="021b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="021b9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="021b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="021b9-107">Criar um novo objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="021b9-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="021b9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="021b9-108">Prerequisites</span></span>
<span data-ttu-id="021b9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="021b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="021b9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="021b9-111">Permission type</span></span>|<span data-ttu-id="021b9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="021b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="021b9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="021b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="021b9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="021b9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="021b9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="021b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="021b9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="021b9-116">Not supported.</span></span>|
|<span data-ttu-id="021b9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="021b9-117">Application</span></span>|<span data-ttu-id="021b9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="021b9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="021b9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="021b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="021b9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="021b9-120">Request headers</span></span>
|<span data-ttu-id="021b9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="021b9-121">Header</span></span>|<span data-ttu-id="021b9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="021b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="021b9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="021b9-123">Authorization</span></span>|<span data-ttu-id="021b9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="021b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="021b9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="021b9-125">Accept</span></span>|<span data-ttu-id="021b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="021b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="021b9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="021b9-127">Request body</span></span>
<span data-ttu-id="021b9-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="021b9-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="021b9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="021b9-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="021b9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="021b9-130">Property</span></span>|<span data-ttu-id="021b9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="021b9-131">Type</span></span>|<span data-ttu-id="021b9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="021b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="021b9-133">id</span><span class="sxs-lookup"><span data-stu-id="021b9-133">id</span></span>|<span data-ttu-id="021b9-134">String</span><span class="sxs-lookup"><span data-stu-id="021b9-134">String</span></span>|<span data-ttu-id="021b9-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="021b9-135">Key of the entity.</span></span> <span data-ttu-id="021b9-136">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="021b9-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="021b9-137">destino</span><span class="sxs-lookup"><span data-stu-id="021b9-137">target</span></span>|[<span data-ttu-id="021b9-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="021b9-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="021b9-139">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="021b9-139">The assignment target for eBook.</span></span> <span data-ttu-id="021b9-140">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="021b9-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="021b9-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="021b9-141">installIntent</span></span>|[<span data-ttu-id="021b9-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="021b9-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="021b9-143">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="021b9-143">The install intent for eBook.</span></span> <span data-ttu-id="021b9-144">Herdada do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="021b9-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="021b9-145">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="021b9-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="021b9-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="021b9-146">Response</span></span>
<span data-ttu-id="021b9-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="021b9-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="021b9-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="021b9-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="021b9-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="021b9-149">Request</span></span>
<span data-ttu-id="021b9-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="021b9-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="021b9-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="021b9-151">Response</span></span>
<span data-ttu-id="021b9-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="021b9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




