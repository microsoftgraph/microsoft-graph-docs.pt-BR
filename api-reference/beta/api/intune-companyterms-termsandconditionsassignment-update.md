---
title: Atualizar termsAndConditionsAssignment
description: Atualizar as propriedades de um objeto termsAndConditionsAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c4de7d4c55d0fc92e7439843f295a08f2ab04515
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170431"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="d07cf-103">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d07cf-103">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="d07cf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d07cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d07cf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d07cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d07cf-106">Atualizar as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d07cf-106">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d07cf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d07cf-107">Prerequisites</span></span>
<span data-ttu-id="d07cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d07cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d07cf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d07cf-110">Permission type</span></span>|<span data-ttu-id="d07cf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d07cf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d07cf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d07cf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d07cf-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d07cf-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d07cf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d07cf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d07cf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d07cf-115">Not supported.</span></span>|
|<span data-ttu-id="d07cf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d07cf-116">Application</span></span>|<span data-ttu-id="d07cf-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d07cf-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d07cf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d07cf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d07cf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d07cf-119">Request headers</span></span>
|<span data-ttu-id="d07cf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d07cf-120">Header</span></span>|<span data-ttu-id="d07cf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d07cf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d07cf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d07cf-122">Authorization</span></span>|<span data-ttu-id="d07cf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d07cf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d07cf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d07cf-124">Accept</span></span>|<span data-ttu-id="d07cf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d07cf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d07cf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d07cf-126">Request body</span></span>
<span data-ttu-id="d07cf-127">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d07cf-127">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="d07cf-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d07cf-128">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="d07cf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d07cf-129">Property</span></span>|<span data-ttu-id="d07cf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d07cf-130">Type</span></span>|<span data-ttu-id="d07cf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d07cf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d07cf-132">id</span><span class="sxs-lookup"><span data-stu-id="d07cf-132">id</span></span>|<span data-ttu-id="d07cf-133">String</span><span class="sxs-lookup"><span data-stu-id="d07cf-133">String</span></span>|<span data-ttu-id="d07cf-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="d07cf-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d07cf-135">destino</span><span class="sxs-lookup"><span data-stu-id="d07cf-135">target</span></span>|[<span data-ttu-id="d07cf-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d07cf-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d07cf-137">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="d07cf-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="d07cf-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d07cf-138">Response</span></span>
<span data-ttu-id="d07cf-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d07cf-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d07cf-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d07cf-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="d07cf-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d07cf-141">Request</span></span>
<span data-ttu-id="d07cf-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d07cf-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d07cf-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d07cf-143">Response</span></span>
<span data-ttu-id="d07cf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d07cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




