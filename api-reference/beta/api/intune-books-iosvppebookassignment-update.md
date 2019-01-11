---
title: Atualizar iosVppEBookAssignment
description: Atualizar as propriedades de um objeto iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e9abf92f2af9ed0a674f7186ee6ebd2433c9e7a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892341"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="de25b-103">Atualizar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="de25b-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="de25b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="de25b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de25b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="de25b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de25b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="de25b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de25b-107">Atualizar as propriedades de um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de25b-107">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de25b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de25b-108">Prerequisites</span></span>
<span data-ttu-id="de25b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de25b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de25b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de25b-111">Permission type</span></span>|<span data-ttu-id="de25b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de25b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de25b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de25b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de25b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de25b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="de25b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de25b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de25b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de25b-116">Not supported.</span></span>|
|<span data-ttu-id="de25b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de25b-117">Application</span></span>|<span data-ttu-id="de25b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de25b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de25b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de25b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="de25b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de25b-120">Request headers</span></span>
|<span data-ttu-id="de25b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de25b-121">Header</span></span>|<span data-ttu-id="de25b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="de25b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de25b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="de25b-123">Authorization</span></span>|<span data-ttu-id="de25b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de25b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de25b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de25b-125">Accept</span></span>|<span data-ttu-id="de25b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de25b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de25b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de25b-127">Request body</span></span>
<span data-ttu-id="de25b-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de25b-128">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="de25b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de25b-129">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="de25b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de25b-130">Property</span></span>|<span data-ttu-id="de25b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="de25b-131">Type</span></span>|<span data-ttu-id="de25b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="de25b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de25b-133">id</span><span class="sxs-lookup"><span data-stu-id="de25b-133">id</span></span>|<span data-ttu-id="de25b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de25b-134">String</span></span>|<span data-ttu-id="de25b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="de25b-135">Key of the entity.</span></span> <span data-ttu-id="de25b-136">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="de25b-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="de25b-137">destino</span><span class="sxs-lookup"><span data-stu-id="de25b-137">target</span></span>|[<span data-ttu-id="de25b-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="de25b-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="de25b-139">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="de25b-139">The assignment target for eBook.</span></span> <span data-ttu-id="de25b-140">Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="de25b-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="de25b-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="de25b-141">installIntent</span></span>|[<span data-ttu-id="de25b-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="de25b-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="de25b-143">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="de25b-143">The install intent for eBook.</span></span> <span data-ttu-id="de25b-144">Herdada do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de25b-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="de25b-145">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="de25b-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="de25b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="de25b-146">Response</span></span>
<span data-ttu-id="de25b-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de25b-147">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de25b-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de25b-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="de25b-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de25b-149">Request</span></span>
<span data-ttu-id="de25b-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de25b-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="de25b-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="de25b-151">Response</span></span>
<span data-ttu-id="de25b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de25b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





