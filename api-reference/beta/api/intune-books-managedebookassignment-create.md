---
title: Criar managedEBookAssignment
description: Criar um novo objeto managedEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ad6d30b07bd128572500be7a1a85fa4ae1333e6c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935203"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="1fe37-103">Criar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="1fe37-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="1fe37-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1fe37-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1fe37-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1fe37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1fe37-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1fe37-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1fe37-107">Criar um novo objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1fe37-107">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1fe37-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1fe37-108">Prerequisites</span></span>
<span data-ttu-id="1fe37-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fe37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fe37-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fe37-111">Permission type</span></span>|<span data-ttu-id="1fe37-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1fe37-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fe37-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fe37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1fe37-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fe37-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1fe37-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fe37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fe37-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fe37-116">Not supported.</span></span>|
|<span data-ttu-id="1fe37-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fe37-117">Application</span></span>|<span data-ttu-id="1fe37-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fe37-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fe37-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fe37-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1fe37-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fe37-120">Request headers</span></span>
|<span data-ttu-id="1fe37-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1fe37-121">Header</span></span>|<span data-ttu-id="1fe37-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1fe37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fe37-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fe37-123">Authorization</span></span>|<span data-ttu-id="1fe37-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fe37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fe37-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1fe37-125">Accept</span></span>|<span data-ttu-id="1fe37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1fe37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fe37-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fe37-127">Request body</span></span>
<span data-ttu-id="1fe37-128">No corpo da solicitação, forneça uma representação JSON do objeto managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="1fe37-128">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="1fe37-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="1fe37-129">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="1fe37-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fe37-130">Property</span></span>|<span data-ttu-id="1fe37-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fe37-131">Type</span></span>|<span data-ttu-id="1fe37-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fe37-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fe37-133">id</span><span class="sxs-lookup"><span data-stu-id="1fe37-133">id</span></span>|<span data-ttu-id="1fe37-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1fe37-134">String</span></span>|<span data-ttu-id="1fe37-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1fe37-135">Key of the entity.</span></span>|
|<span data-ttu-id="1fe37-136">destino</span><span class="sxs-lookup"><span data-stu-id="1fe37-136">target</span></span>|[<span data-ttu-id="1fe37-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1fe37-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1fe37-138">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="1fe37-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="1fe37-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="1fe37-139">installIntent</span></span>|[<span data-ttu-id="1fe37-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="1fe37-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="1fe37-141">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="1fe37-141">The install intent for eBook.</span></span> <span data-ttu-id="1fe37-142">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="1fe37-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="1fe37-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fe37-143">Response</span></span>
<span data-ttu-id="1fe37-144">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fe37-144">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fe37-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1fe37-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="1fe37-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fe37-146">Request</span></span>
<span data-ttu-id="1fe37-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fe37-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="1fe37-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fe37-148">Response</span></span>
<span data-ttu-id="1fe37-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1fe37-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





