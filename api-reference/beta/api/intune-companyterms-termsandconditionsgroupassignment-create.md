---
title: Criar termsAndConditionsGroupAssignment
description: Criar um novo objeto termsAndConditionsGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9c055f2a8d5d29da58ace22fd7a9f8722cef2510
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170417"
---
# <a name="create-termsandconditionsgroupassignment"></a><span data-ttu-id="a929a-103">Criar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a929a-103">Create termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="a929a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a929a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a929a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a929a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a929a-106">Criar um novo objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a929a-106">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a929a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a929a-107">Prerequisites</span></span>
<span data-ttu-id="a929a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a929a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a929a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a929a-110">Permission type</span></span>|<span data-ttu-id="a929a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a929a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a929a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a929a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a929a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a929a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a929a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a929a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a929a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a929a-115">Not supported.</span></span>|
|<span data-ttu-id="a929a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a929a-116">Application</span></span>|<span data-ttu-id="a929a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a929a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a929a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a929a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a929a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a929a-119">Request headers</span></span>
|<span data-ttu-id="a929a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a929a-120">Header</span></span>|<span data-ttu-id="a929a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a929a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a929a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a929a-122">Authorization</span></span>|<span data-ttu-id="a929a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a929a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a929a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a929a-124">Accept</span></span>|<span data-ttu-id="a929a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a929a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a929a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a929a-126">Request body</span></span>
<span data-ttu-id="a929a-127">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditionsGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="a929a-127">In the request body, supply a JSON representation for the termsAndConditionsGroupAssignment object.</span></span>

<span data-ttu-id="a929a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditionsGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="a929a-128">The following table shows the properties that are required when you create the termsAndConditionsGroupAssignment.</span></span>

|<span data-ttu-id="a929a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a929a-129">Property</span></span>|<span data-ttu-id="a929a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a929a-130">Type</span></span>|<span data-ttu-id="a929a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a929a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a929a-132">id</span><span class="sxs-lookup"><span data-stu-id="a929a-132">id</span></span>|<span data-ttu-id="a929a-133">String</span><span class="sxs-lookup"><span data-stu-id="a929a-133">String</span></span>|<span data-ttu-id="a929a-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="a929a-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="a929a-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="a929a-135">targetGroupId</span></span>|<span data-ttu-id="a929a-136">String</span><span class="sxs-lookup"><span data-stu-id="a929a-136">String</span></span>|<span data-ttu-id="a929a-137">Identificador exclusivo de um grupo ao qual a política T&C é atribuída.</span><span class="sxs-lookup"><span data-stu-id="a929a-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="a929a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a929a-138">Response</span></span>
<span data-ttu-id="a929a-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a929a-139">If successful, this method returns a `201 Created` response code and a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a929a-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a929a-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a929a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a929a-141">Request</span></span>
<span data-ttu-id="a929a-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a929a-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="a929a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a929a-143">Response</span></span>
<span data-ttu-id="a929a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a929a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 169

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
  "targetGroupId": "Target Group Id value"
}
```




