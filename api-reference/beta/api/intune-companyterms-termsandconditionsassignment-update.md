---
title: Atualizar termsAndConditionsAssignment
description: Atualizar as propriedades de um objeto termsAndConditionsAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26abb6510ac5c76a950858a1b3b76d3e79e3056f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156578"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="8543e-103">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="8543e-103">Update termsAndConditionsAssignment</span></span>

<span data-ttu-id="8543e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8543e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8543e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8543e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8543e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8543e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8543e-107">Atualizar as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8543e-107">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8543e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8543e-108">Prerequisites</span></span>
<span data-ttu-id="8543e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8543e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8543e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8543e-111">Permission type</span></span>|<span data-ttu-id="8543e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8543e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8543e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8543e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8543e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8543e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8543e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8543e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8543e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8543e-116">Not supported.</span></span>|
|<span data-ttu-id="8543e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8543e-117">Application</span></span>|<span data-ttu-id="8543e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8543e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8543e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8543e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8543e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8543e-120">Request headers</span></span>
|<span data-ttu-id="8543e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8543e-121">Header</span></span>|<span data-ttu-id="8543e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8543e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8543e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8543e-123">Authorization</span></span>|<span data-ttu-id="8543e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8543e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8543e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8543e-125">Accept</span></span>|<span data-ttu-id="8543e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8543e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8543e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8543e-127">Request body</span></span>
<span data-ttu-id="8543e-128">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8543e-128">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="8543e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8543e-129">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="8543e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8543e-130">Property</span></span>|<span data-ttu-id="8543e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8543e-131">Type</span></span>|<span data-ttu-id="8543e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8543e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8543e-133">id</span><span class="sxs-lookup"><span data-stu-id="8543e-133">id</span></span>|<span data-ttu-id="8543e-134">String</span><span class="sxs-lookup"><span data-stu-id="8543e-134">String</span></span>|<span data-ttu-id="8543e-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="8543e-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="8543e-136">destino</span><span class="sxs-lookup"><span data-stu-id="8543e-136">target</span></span>|[<span data-ttu-id="8543e-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8543e-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8543e-138">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="8543e-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="8543e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8543e-139">Response</span></span>
<span data-ttu-id="8543e-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8543e-140">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8543e-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8543e-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="8543e-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8543e-142">Request</span></span>
<span data-ttu-id="8543e-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8543e-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 387

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="8543e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8543e-144">Response</span></span>
<span data-ttu-id="8543e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8543e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 436

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




