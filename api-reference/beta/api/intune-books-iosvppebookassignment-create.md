---
title: Criar iosVppEBookAssignment
description: Criar um novo objeto iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b5ff460b702c943268d9992bd17e99fd54369548
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963966"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="5e09c-103">Criar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="5e09c-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="5e09c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5e09c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e09c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5e09c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e09c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5e09c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e09c-107">Criar um novo objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5e09c-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5e09c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e09c-108">Prerequisites</span></span>
<span data-ttu-id="5e09c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e09c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e09c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e09c-111">Permission type</span></span>|<span data-ttu-id="5e09c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5e09c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e09c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e09c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e09c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e09c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5e09c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e09c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e09c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e09c-116">Not supported.</span></span>|
|<span data-ttu-id="5e09c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e09c-117">Application</span></span>|<span data-ttu-id="5e09c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e09c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e09c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e09c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="5e09c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e09c-120">Request headers</span></span>
|<span data-ttu-id="5e09c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e09c-121">Header</span></span>|<span data-ttu-id="5e09c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5e09c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e09c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e09c-123">Authorization</span></span>|<span data-ttu-id="5e09c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e09c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e09c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5e09c-125">Accept</span></span>|<span data-ttu-id="5e09c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e09c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e09c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e09c-127">Request body</span></span>
<span data-ttu-id="5e09c-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="5e09c-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="5e09c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="5e09c-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="5e09c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e09c-130">Property</span></span>|<span data-ttu-id="5e09c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e09c-131">Type</span></span>|<span data-ttu-id="5e09c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e09c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e09c-133">id</span><span class="sxs-lookup"><span data-stu-id="5e09c-133">id</span></span>|<span data-ttu-id="5e09c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e09c-134">String</span></span>|<span data-ttu-id="5e09c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5e09c-135">Key of the entity.</span></span> <span data-ttu-id="5e09c-136">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5e09c-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="5e09c-137">destino</span><span class="sxs-lookup"><span data-stu-id="5e09c-137">target</span></span>|[<span data-ttu-id="5e09c-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5e09c-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5e09c-139">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="5e09c-139">The assignment target for eBook.</span></span> <span data-ttu-id="5e09c-140">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5e09c-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="5e09c-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="5e09c-141">installIntent</span></span>|[<span data-ttu-id="5e09c-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="5e09c-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="5e09c-143">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="5e09c-143">The install intent for eBook.</span></span> <span data-ttu-id="5e09c-144">Herdada do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5e09c-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="5e09c-145">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="5e09c-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="5e09c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e09c-146">Response</span></span>
<span data-ttu-id="5e09c-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e09c-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e09c-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e09c-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e09c-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e09c-149">Request</span></span>
<span data-ttu-id="5e09c-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e09c-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5e09c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e09c-151">Response</span></span>
<span data-ttu-id="5e09c-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e09c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





