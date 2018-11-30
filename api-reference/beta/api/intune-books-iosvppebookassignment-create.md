---
title: Criar iosVppEBookAssignment
description: Criar um novo objeto iosVppEBookAssignment.
ms.openlocfilehash: 192f5e006fa89f3dbf25a320967af68fbd06f7ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038407"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="51fd7-103">Criar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="51fd7-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="51fd7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="51fd7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51fd7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="51fd7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51fd7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="51fd7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51fd7-107">Criar um novo objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="51fd7-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51fd7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51fd7-108">Prerequisites</span></span>
<span data-ttu-id="51fd7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51fd7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51fd7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51fd7-111">Permission type</span></span>|<span data-ttu-id="51fd7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51fd7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51fd7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51fd7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51fd7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51fd7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51fd7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51fd7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51fd7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51fd7-116">Not supported.</span></span>|
|<span data-ttu-id="51fd7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51fd7-117">Application</span></span>|<span data-ttu-id="51fd7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51fd7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51fd7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51fd7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="51fd7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51fd7-120">Request headers</span></span>
|<span data-ttu-id="51fd7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51fd7-121">Header</span></span>|<span data-ttu-id="51fd7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="51fd7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51fd7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="51fd7-123">Authorization</span></span>|<span data-ttu-id="51fd7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51fd7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51fd7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51fd7-125">Accept</span></span>|<span data-ttu-id="51fd7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51fd7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51fd7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51fd7-127">Request body</span></span>
<span data-ttu-id="51fd7-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="51fd7-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="51fd7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="51fd7-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="51fd7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51fd7-130">Property</span></span>|<span data-ttu-id="51fd7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="51fd7-131">Type</span></span>|<span data-ttu-id="51fd7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="51fd7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51fd7-133">id</span><span class="sxs-lookup"><span data-stu-id="51fd7-133">id</span></span>|<span data-ttu-id="51fd7-134">String</span><span class="sxs-lookup"><span data-stu-id="51fd7-134">String</span></span>|<span data-ttu-id="51fd7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="51fd7-135">Key of the entity.</span></span> <span data-ttu-id="51fd7-136">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="51fd7-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="51fd7-137">destino</span><span class="sxs-lookup"><span data-stu-id="51fd7-137">target</span></span>|[<span data-ttu-id="51fd7-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="51fd7-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="51fd7-139">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="51fd7-139">The assignment target for eBook.</span></span> <span data-ttu-id="51fd7-140">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="51fd7-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="51fd7-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="51fd7-141">installIntent</span></span>|[<span data-ttu-id="51fd7-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="51fd7-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="51fd7-143">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="51fd7-143">The install intent for eBook.</span></span> <span data-ttu-id="51fd7-144">Herdada do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="51fd7-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="51fd7-145">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="51fd7-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="51fd7-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="51fd7-146">Response</span></span>
<span data-ttu-id="51fd7-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51fd7-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51fd7-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51fd7-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="51fd7-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51fd7-149">Request</span></span>
<span data-ttu-id="51fd7-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51fd7-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="51fd7-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="51fd7-151">Response</span></span>
<span data-ttu-id="51fd7-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51fd7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





