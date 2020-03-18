---
title: Criar termsAndConditionsGroupAssignment
description: Criar um novo objeto termsAndConditionsGroupAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ebb289d651037d830bb9d4c58f21672154c5d257
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760071"
---
# <a name="create-termsandconditionsgroupassignment"></a><span data-ttu-id="74f78-103">Criar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="74f78-103">Create termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="74f78-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="74f78-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74f78-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="74f78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74f78-106">Criar um novo objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="74f78-106">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74f78-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="74f78-107">Prerequisites</span></span>
<span data-ttu-id="74f78-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74f78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74f78-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74f78-110">Permission type</span></span>|<span data-ttu-id="74f78-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="74f78-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74f78-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74f78-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74f78-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74f78-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="74f78-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74f78-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74f78-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74f78-115">Not supported.</span></span>|
|<span data-ttu-id="74f78-116">Application</span><span class="sxs-lookup"><span data-stu-id="74f78-116">Application</span></span>|<span data-ttu-id="74f78-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74f78-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74f78-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74f78-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="74f78-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74f78-119">Request headers</span></span>
|<span data-ttu-id="74f78-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74f78-120">Header</span></span>|<span data-ttu-id="74f78-121">Valor</span><span class="sxs-lookup"><span data-stu-id="74f78-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74f78-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="74f78-122">Authorization</span></span>|<span data-ttu-id="74f78-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74f78-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74f78-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="74f78-124">Accept</span></span>|<span data-ttu-id="74f78-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74f78-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74f78-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74f78-126">Request body</span></span>
<span data-ttu-id="74f78-127">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditionsGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="74f78-127">In the request body, supply a JSON representation for the termsAndConditionsGroupAssignment object.</span></span>

<span data-ttu-id="74f78-128">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditionsGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="74f78-128">The following table shows the properties that are required when you create the termsAndConditionsGroupAssignment.</span></span>

|<span data-ttu-id="74f78-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74f78-129">Property</span></span>|<span data-ttu-id="74f78-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="74f78-130">Type</span></span>|<span data-ttu-id="74f78-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="74f78-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74f78-132">id</span><span class="sxs-lookup"><span data-stu-id="74f78-132">id</span></span>|<span data-ttu-id="74f78-133">String</span><span class="sxs-lookup"><span data-stu-id="74f78-133">String</span></span>|<span data-ttu-id="74f78-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="74f78-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="74f78-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="74f78-135">targetGroupId</span></span>|<span data-ttu-id="74f78-136">String</span><span class="sxs-lookup"><span data-stu-id="74f78-136">String</span></span>|<span data-ttu-id="74f78-137">Identificador exclusivo de um grupo ao qual a política T&C é atribuída.</span><span class="sxs-lookup"><span data-stu-id="74f78-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="74f78-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="74f78-138">Response</span></span>
<span data-ttu-id="74f78-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74f78-139">If successful, this method returns a `201 Created` response code and a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74f78-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74f78-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="74f78-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74f78-141">Request</span></span>
<span data-ttu-id="74f78-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74f78-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="74f78-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="74f78-143">Response</span></span>
<span data-ttu-id="74f78-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74f78-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




