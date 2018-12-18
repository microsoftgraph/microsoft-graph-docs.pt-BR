---
title: Atualizar termsAndConditionsAssignment
description: Atualizar as propriedades de um objeto termsAndConditionsAssignment.
author: tfitzmac
ms.openlocfilehash: b55ec01c6bac55f9b1d72a5aad5f931bed6b6b2a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301404"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="ad384-103">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ad384-103">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="ad384-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ad384-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad384-105">Atualizar as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ad384-105">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad384-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ad384-106">Prerequisites</span></span>
<span data-ttu-id="ad384-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad384-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad384-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad384-109">Permission type</span></span>|<span data-ttu-id="ad384-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ad384-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad384-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad384-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ad384-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad384-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ad384-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad384-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad384-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad384-114">Not supported.</span></span>|
|<span data-ttu-id="ad384-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad384-115">Application</span></span>|<span data-ttu-id="ad384-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad384-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad384-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad384-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ad384-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad384-118">Request headers</span></span>
|<span data-ttu-id="ad384-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad384-119">Header</span></span>|<span data-ttu-id="ad384-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ad384-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad384-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad384-121">Authorization</span></span>|<span data-ttu-id="ad384-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad384-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad384-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ad384-123">Accept</span></span>|<span data-ttu-id="ad384-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ad384-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad384-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad384-125">Request body</span></span>
<span data-ttu-id="ad384-126">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ad384-126">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="ad384-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ad384-127">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="ad384-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad384-128">Property</span></span>|<span data-ttu-id="ad384-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad384-129">Type</span></span>|<span data-ttu-id="ad384-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad384-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad384-131">id</span><span class="sxs-lookup"><span data-stu-id="ad384-131">id</span></span>|<span data-ttu-id="ad384-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad384-132">String</span></span>|<span data-ttu-id="ad384-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="ad384-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ad384-134">destino</span><span class="sxs-lookup"><span data-stu-id="ad384-134">target</span></span>|[<span data-ttu-id="ad384-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ad384-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ad384-136">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="ad384-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="ad384-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad384-137">Response</span></span>
<span data-ttu-id="ad384-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad384-138">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad384-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad384-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad384-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad384-140">Request</span></span>
<span data-ttu-id="ad384-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad384-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ad384-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad384-142">Response</span></span>
<span data-ttu-id="ad384-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad384-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



