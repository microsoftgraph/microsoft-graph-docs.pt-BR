---
title: Criar termsAndConditionsAssignment
description: Criar um novo objeto termsAndConditionsAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 329bd5b227600dff42c96d54a6a0497f8b978af3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760106"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="86631-103">Criar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="86631-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="86631-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86631-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86631-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86631-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86631-106">Criar um novo objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="86631-106">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86631-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86631-107">Prerequisites</span></span>
<span data-ttu-id="86631-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86631-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86631-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86631-110">Permission type</span></span>|<span data-ttu-id="86631-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86631-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86631-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86631-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86631-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86631-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="86631-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86631-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86631-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86631-115">Not supported.</span></span>|
|<span data-ttu-id="86631-116">Application</span><span class="sxs-lookup"><span data-stu-id="86631-116">Application</span></span>|<span data-ttu-id="86631-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86631-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86631-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86631-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="86631-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86631-119">Request headers</span></span>
|<span data-ttu-id="86631-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86631-120">Header</span></span>|<span data-ttu-id="86631-121">Valor</span><span class="sxs-lookup"><span data-stu-id="86631-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86631-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="86631-122">Authorization</span></span>|<span data-ttu-id="86631-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86631-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86631-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86631-124">Accept</span></span>|<span data-ttu-id="86631-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86631-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86631-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86631-126">Request body</span></span>
<span data-ttu-id="86631-127">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditionsAssignment.</span><span class="sxs-lookup"><span data-stu-id="86631-127">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="86631-128">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditionsAssignment.</span><span class="sxs-lookup"><span data-stu-id="86631-128">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="86631-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86631-129">Property</span></span>|<span data-ttu-id="86631-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="86631-130">Type</span></span>|<span data-ttu-id="86631-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="86631-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86631-132">id</span><span class="sxs-lookup"><span data-stu-id="86631-132">id</span></span>|<span data-ttu-id="86631-133">String</span><span class="sxs-lookup"><span data-stu-id="86631-133">String</span></span>|<span data-ttu-id="86631-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="86631-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="86631-135">destino</span><span class="sxs-lookup"><span data-stu-id="86631-135">target</span></span>|[<span data-ttu-id="86631-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="86631-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="86631-137">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="86631-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="86631-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="86631-138">Response</span></span>
<span data-ttu-id="86631-139">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86631-139">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86631-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86631-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="86631-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86631-141">Request</span></span>
<span data-ttu-id="86631-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86631-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="86631-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="86631-143">Response</span></span>
<span data-ttu-id="86631-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86631-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




