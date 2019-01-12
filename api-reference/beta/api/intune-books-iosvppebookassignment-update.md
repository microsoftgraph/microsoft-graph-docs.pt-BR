---
title: Atualizar iosVppEBookAssignment
description: Atualizar as propriedades de um objeto iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 272de2b88b930b8f55849e6a791dce6c77d1595c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958373"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="ad3ec-103">Atualizar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="ad3ec-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="ad3ec-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ad3ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad3ec-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ad3ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad3ec-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ad3ec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad3ec-107">Atualizar as propriedades de um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ad3ec-107">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad3ec-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ad3ec-108">Prerequisites</span></span>
<span data-ttu-id="ad3ec-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad3ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad3ec-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad3ec-111">Permission type</span></span>|<span data-ttu-id="ad3ec-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ad3ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad3ec-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad3ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad3ec-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad3ec-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ad3ec-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad3ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad3ec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad3ec-116">Not supported.</span></span>|
|<span data-ttu-id="ad3ec-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad3ec-117">Application</span></span>|<span data-ttu-id="ad3ec-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad3ec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad3ec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad3ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ad3ec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad3ec-120">Request headers</span></span>
|<span data-ttu-id="ad3ec-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad3ec-121">Header</span></span>|<span data-ttu-id="ad3ec-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ad3ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad3ec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad3ec-123">Authorization</span></span>|<span data-ttu-id="ad3ec-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad3ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad3ec-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ad3ec-125">Accept</span></span>|<span data-ttu-id="ad3ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad3ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad3ec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad3ec-127">Request body</span></span>
<span data-ttu-id="ad3ec-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ad3ec-128">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="ad3ec-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ad3ec-129">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="ad3ec-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad3ec-130">Property</span></span>|<span data-ttu-id="ad3ec-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad3ec-131">Type</span></span>|<span data-ttu-id="ad3ec-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad3ec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad3ec-133">id</span><span class="sxs-lookup"><span data-stu-id="ad3ec-133">id</span></span>|<span data-ttu-id="ad3ec-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad3ec-134">String</span></span>|<span data-ttu-id="ad3ec-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ad3ec-135">Key of the entity.</span></span> <span data-ttu-id="ad3ec-136">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ad3ec-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="ad3ec-137">destino</span><span class="sxs-lookup"><span data-stu-id="ad3ec-137">target</span></span>|[<span data-ttu-id="ad3ec-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ad3ec-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ad3ec-139">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="ad3ec-139">The assignment target for eBook.</span></span> <span data-ttu-id="ad3ec-140">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ad3ec-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="ad3ec-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="ad3ec-141">installIntent</span></span>|[<span data-ttu-id="ad3ec-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="ad3ec-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="ad3ec-143">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="ad3ec-143">The install intent for eBook.</span></span> <span data-ttu-id="ad3ec-144">Herdada do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ad3ec-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="ad3ec-145">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="ad3ec-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="ad3ec-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad3ec-146">Response</span></span>
<span data-ttu-id="ad3ec-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad3ec-147">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad3ec-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad3ec-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad3ec-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad3ec-149">Request</span></span>
<span data-ttu-id="ad3ec-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad3ec-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 133

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="ad3ec-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad3ec-151">Response</span></span>
<span data-ttu-id="ad3ec-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad3ec-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





