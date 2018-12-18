---
title: Atualizar iosVppEBookAssignment
description: Atualizar as propriedades de um objeto iosVppEBookAssignment.
author: tfitzmac
ms.openlocfilehash: 537c2ef5838dc68881f3de693a6591570219ece4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338147"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="7d720-103">Atualizar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="7d720-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="7d720-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7d720-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d720-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7d720-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d720-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7d720-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d720-107">Atualizar as propriedades de um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7d720-107">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d720-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d720-108">Prerequisites</span></span>
<span data-ttu-id="7d720-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d720-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d720-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d720-111">Permission type</span></span>|<span data-ttu-id="7d720-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d720-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d720-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d720-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d720-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d720-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7d720-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d720-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d720-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d720-116">Not supported.</span></span>|
|<span data-ttu-id="7d720-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d720-117">Application</span></span>|<span data-ttu-id="7d720-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d720-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d720-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d720-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7d720-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d720-120">Request headers</span></span>
|<span data-ttu-id="7d720-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d720-121">Header</span></span>|<span data-ttu-id="7d720-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7d720-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d720-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d720-123">Authorization</span></span>|<span data-ttu-id="7d720-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d720-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d720-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d720-125">Accept</span></span>|<span data-ttu-id="7d720-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d720-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d720-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d720-127">Request body</span></span>
<span data-ttu-id="7d720-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7d720-128">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="7d720-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7d720-129">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="7d720-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d720-130">Property</span></span>|<span data-ttu-id="7d720-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d720-131">Type</span></span>|<span data-ttu-id="7d720-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d720-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d720-133">id</span><span class="sxs-lookup"><span data-stu-id="7d720-133">id</span></span>|<span data-ttu-id="7d720-134">String</span><span class="sxs-lookup"><span data-stu-id="7d720-134">String</span></span>|<span data-ttu-id="7d720-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7d720-135">Key of the entity.</span></span> <span data-ttu-id="7d720-136">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7d720-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="7d720-137">destino</span><span class="sxs-lookup"><span data-stu-id="7d720-137">target</span></span>|[<span data-ttu-id="7d720-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7d720-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7d720-139">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="7d720-139">The assignment target for eBook.</span></span> <span data-ttu-id="7d720-140">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7d720-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="7d720-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="7d720-141">installIntent</span></span>|[<span data-ttu-id="7d720-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="7d720-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="7d720-143">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="7d720-143">The install intent for eBook.</span></span> <span data-ttu-id="7d720-144">Herdada do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7d720-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="7d720-145">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="7d720-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="7d720-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d720-146">Response</span></span>
<span data-ttu-id="7d720-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d720-147">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d720-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d720-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="7d720-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d720-149">Request</span></span>
<span data-ttu-id="7d720-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d720-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d720-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d720-151">Response</span></span>
<span data-ttu-id="7d720-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d720-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





