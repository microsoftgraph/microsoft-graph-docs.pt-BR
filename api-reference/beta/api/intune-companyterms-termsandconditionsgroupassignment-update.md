---
title: Atualizar termsAndConditionsGroupAssignment
description: Atualiza as propriedades de um objeto termsAndConditionsGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d76b67f72b18ed29cc98c4bad7c9c035b4ee01ca
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975879"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="c55b4-103">Atualizar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="c55b4-103">Update termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="c55b4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c55b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c55b4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c55b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c55b4-106">Atualiza as propriedades de um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c55b4-106">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c55b4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c55b4-107">Prerequisites</span></span>
<span data-ttu-id="c55b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c55b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c55b4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c55b4-110">Permission type</span></span>|<span data-ttu-id="c55b4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c55b4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c55b4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c55b4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c55b4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c55b4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c55b4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c55b4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c55b4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c55b4-115">Not supported.</span></span>|
|<span data-ttu-id="c55b4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c55b4-116">Application</span></span>|<span data-ttu-id="c55b4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c55b4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c55b4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c55b4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c55b4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c55b4-119">Request headers</span></span>
|<span data-ttu-id="c55b4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c55b4-120">Header</span></span>|<span data-ttu-id="c55b4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c55b4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c55b4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c55b4-122">Authorization</span></span>|<span data-ttu-id="c55b4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c55b4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c55b4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c55b4-124">Accept</span></span>|<span data-ttu-id="c55b4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c55b4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c55b4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c55b4-126">Request body</span></span>
<span data-ttu-id="c55b4-127">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c55b4-127">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="c55b4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c55b4-128">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="c55b4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c55b4-129">Property</span></span>|<span data-ttu-id="c55b4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c55b4-130">Type</span></span>|<span data-ttu-id="c55b4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c55b4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c55b4-132">id</span><span class="sxs-lookup"><span data-stu-id="c55b4-132">id</span></span>|<span data-ttu-id="c55b4-133">String</span><span class="sxs-lookup"><span data-stu-id="c55b4-133">String</span></span>|<span data-ttu-id="c55b4-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="c55b4-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="c55b4-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="c55b4-135">targetGroupId</span></span>|<span data-ttu-id="c55b4-136">String</span><span class="sxs-lookup"><span data-stu-id="c55b4-136">String</span></span>|<span data-ttu-id="c55b4-137">Identificador exclusivo de um grupo ao qual a política T&C é atribuída.</span><span class="sxs-lookup"><span data-stu-id="c55b4-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="c55b4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c55b4-138">Response</span></span>
<span data-ttu-id="c55b4-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c55b4-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c55b4-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c55b4-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="c55b4-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c55b4-141">Request</span></span>
<span data-ttu-id="c55b4-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c55b4-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="c55b4-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c55b4-143">Response</span></span>
<span data-ttu-id="c55b4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c55b4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




