---
title: Atualizar termsAndConditionsGroupAssignment
description: Atualiza as propriedades de um objeto termsAndConditionsGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 698e82c83fc1e528b27971aa409cce115bee6315
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436318"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="5ac72-103">Atualizar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="5ac72-103">Update termsAndConditionsGroupAssignment</span></span>

<span data-ttu-id="5ac72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ac72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ac72-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ac72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ac72-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ac72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ac72-107">Atualiza as propriedades de um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5ac72-107">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ac72-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ac72-108">Prerequisites</span></span>
<span data-ttu-id="5ac72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ac72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ac72-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ac72-111">Permission type</span></span>|<span data-ttu-id="5ac72-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ac72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ac72-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ac72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ac72-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ac72-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5ac72-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ac72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ac72-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ac72-116">Not supported.</span></span>|
|<span data-ttu-id="5ac72-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ac72-117">Application</span></span>|<span data-ttu-id="5ac72-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ac72-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ac72-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ac72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5ac72-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ac72-120">Request headers</span></span>
|<span data-ttu-id="5ac72-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ac72-121">Header</span></span>|<span data-ttu-id="5ac72-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5ac72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ac72-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ac72-123">Authorization</span></span>|<span data-ttu-id="5ac72-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ac72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ac72-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ac72-125">Accept</span></span>|<span data-ttu-id="5ac72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ac72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ac72-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ac72-127">Request body</span></span>
<span data-ttu-id="5ac72-128">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5ac72-128">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="5ac72-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5ac72-129">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="5ac72-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ac72-130">Property</span></span>|<span data-ttu-id="5ac72-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ac72-131">Type</span></span>|<span data-ttu-id="5ac72-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ac72-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ac72-133">id</span><span class="sxs-lookup"><span data-stu-id="5ac72-133">id</span></span>|<span data-ttu-id="5ac72-134">String</span><span class="sxs-lookup"><span data-stu-id="5ac72-134">String</span></span>|<span data-ttu-id="5ac72-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ac72-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="5ac72-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="5ac72-136">targetGroupId</span></span>|<span data-ttu-id="5ac72-137">String</span><span class="sxs-lookup"><span data-stu-id="5ac72-137">String</span></span>|<span data-ttu-id="5ac72-138">Identificador exclusivo de um grupo ao qual a política T&C é atribuída.</span><span class="sxs-lookup"><span data-stu-id="5ac72-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="5ac72-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ac72-139">Response</span></span>
<span data-ttu-id="5ac72-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ac72-140">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ac72-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ac72-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ac72-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ac72-142">Request</span></span>
<span data-ttu-id="5ac72-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ac72-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="5ac72-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ac72-144">Response</span></span>
<span data-ttu-id="5ac72-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ac72-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 169

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
  "targetGroupId": "Target Group Id value"
}
```



