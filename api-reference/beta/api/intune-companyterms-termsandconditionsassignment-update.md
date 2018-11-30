---
title: Atualizar termsAndConditionsAssignment
description: Atualizar as propriedades de um objeto termsAndConditionsAssignment.
ms.openlocfilehash: a4c6f54da36593dbda0c552d46cd80c3e24b6261
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033611"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="5714d-103">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="5714d-103">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="5714d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5714d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5714d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5714d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5714d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5714d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5714d-107">Atualizar as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5714d-107">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5714d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5714d-108">Prerequisites</span></span>
<span data-ttu-id="5714d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5714d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5714d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5714d-111">Permission type</span></span>|<span data-ttu-id="5714d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5714d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5714d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5714d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5714d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5714d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5714d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5714d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5714d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5714d-116">Not supported.</span></span>|
|<span data-ttu-id="5714d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5714d-117">Application</span></span>|<span data-ttu-id="5714d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5714d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5714d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5714d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5714d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5714d-120">Request headers</span></span>
|<span data-ttu-id="5714d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5714d-121">Header</span></span>|<span data-ttu-id="5714d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5714d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5714d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5714d-123">Authorization</span></span>|<span data-ttu-id="5714d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5714d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5714d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5714d-125">Accept</span></span>|<span data-ttu-id="5714d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5714d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5714d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5714d-127">Request body</span></span>
<span data-ttu-id="5714d-128">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5714d-128">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="5714d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5714d-129">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="5714d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5714d-130">Property</span></span>|<span data-ttu-id="5714d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5714d-131">Type</span></span>|<span data-ttu-id="5714d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5714d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5714d-133">id</span><span class="sxs-lookup"><span data-stu-id="5714d-133">id</span></span>|<span data-ttu-id="5714d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5714d-134">String</span></span>|<span data-ttu-id="5714d-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="5714d-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="5714d-136">destino</span><span class="sxs-lookup"><span data-stu-id="5714d-136">target</span></span>|[<span data-ttu-id="5714d-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5714d-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5714d-138">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="5714d-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="5714d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5714d-139">Response</span></span>
<span data-ttu-id="5714d-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5714d-140">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5714d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5714d-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="5714d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5714d-142">Request</span></span>
<span data-ttu-id="5714d-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5714d-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="5714d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="5714d-144">Response</span></span>
<span data-ttu-id="5714d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5714d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 217

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





