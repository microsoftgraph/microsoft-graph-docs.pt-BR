---
title: Criar termsAndConditionsAssignment
description: Criar um novo objeto termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: af88847ac2ce47b09f5a07304f02a1d1fcce2598
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786501"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="384a6-103">Criar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="384a6-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="384a6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="384a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="384a6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="384a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="384a6-106">Criar um novo objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="384a6-106">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="384a6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="384a6-107">Prerequisites</span></span>
<span data-ttu-id="384a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="384a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="384a6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="384a6-110">Permission type</span></span>|<span data-ttu-id="384a6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="384a6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="384a6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="384a6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="384a6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="384a6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="384a6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="384a6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="384a6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="384a6-115">Not supported.</span></span>|
|<span data-ttu-id="384a6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="384a6-116">Application</span></span>|<span data-ttu-id="384a6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="384a6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="384a6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="384a6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="384a6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="384a6-119">Request headers</span></span>
|<span data-ttu-id="384a6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="384a6-120">Header</span></span>|<span data-ttu-id="384a6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="384a6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="384a6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="384a6-122">Authorization</span></span>|<span data-ttu-id="384a6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="384a6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="384a6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="384a6-124">Accept</span></span>|<span data-ttu-id="384a6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="384a6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="384a6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="384a6-126">Request body</span></span>
<span data-ttu-id="384a6-127">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditionsAssignment.</span><span class="sxs-lookup"><span data-stu-id="384a6-127">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="384a6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditionsAssignment.</span><span class="sxs-lookup"><span data-stu-id="384a6-128">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="384a6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="384a6-129">Property</span></span>|<span data-ttu-id="384a6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="384a6-130">Type</span></span>|<span data-ttu-id="384a6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="384a6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="384a6-132">id</span><span class="sxs-lookup"><span data-stu-id="384a6-132">id</span></span>|<span data-ttu-id="384a6-133">String</span><span class="sxs-lookup"><span data-stu-id="384a6-133">String</span></span>|<span data-ttu-id="384a6-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="384a6-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="384a6-135">destino</span><span class="sxs-lookup"><span data-stu-id="384a6-135">target</span></span>|[<span data-ttu-id="384a6-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="384a6-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="384a6-137">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="384a6-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="384a6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="384a6-138">Response</span></span>
<span data-ttu-id="384a6-139">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="384a6-139">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="384a6-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="384a6-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="384a6-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="384a6-141">Request</span></span>
<span data-ttu-id="384a6-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="384a6-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="384a6-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="384a6-143">Response</span></span>
<span data-ttu-id="384a6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="384a6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





