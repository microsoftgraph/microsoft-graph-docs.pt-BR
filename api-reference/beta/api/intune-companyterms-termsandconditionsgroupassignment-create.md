---
title: Criar termsAndConditionsGroupAssignment
description: Criar um novo objeto termsAndConditionsGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e57349fb95334fa204b4f5c33b4ae3a3e904b473
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444312"
---
# <a name="create-termsandconditionsgroupassignment"></a><span data-ttu-id="70133-103">Criar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="70133-103">Create termsAndConditionsGroupAssignment</span></span>

<span data-ttu-id="70133-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="70133-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70133-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="70133-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70133-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="70133-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70133-107">Criar um novo objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="70133-107">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70133-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="70133-108">Prerequisites</span></span>
<span data-ttu-id="70133-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70133-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70133-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70133-111">Permission type</span></span>|<span data-ttu-id="70133-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="70133-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70133-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70133-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70133-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70133-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="70133-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70133-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70133-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70133-116">Not supported.</span></span>|
|<span data-ttu-id="70133-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70133-117">Application</span></span>|<span data-ttu-id="70133-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70133-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70133-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70133-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="70133-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70133-120">Request headers</span></span>
|<span data-ttu-id="70133-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="70133-121">Header</span></span>|<span data-ttu-id="70133-122">Valor</span><span class="sxs-lookup"><span data-stu-id="70133-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70133-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="70133-123">Authorization</span></span>|<span data-ttu-id="70133-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70133-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70133-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="70133-125">Accept</span></span>|<span data-ttu-id="70133-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70133-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70133-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70133-127">Request body</span></span>
<span data-ttu-id="70133-128">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditionsGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="70133-128">In the request body, supply a JSON representation for the termsAndConditionsGroupAssignment object.</span></span>

<span data-ttu-id="70133-129">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditionsGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="70133-129">The following table shows the properties that are required when you create the termsAndConditionsGroupAssignment.</span></span>

|<span data-ttu-id="70133-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70133-130">Property</span></span>|<span data-ttu-id="70133-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="70133-131">Type</span></span>|<span data-ttu-id="70133-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="70133-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70133-133">id</span><span class="sxs-lookup"><span data-stu-id="70133-133">id</span></span>|<span data-ttu-id="70133-134">String</span><span class="sxs-lookup"><span data-stu-id="70133-134">String</span></span>|<span data-ttu-id="70133-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="70133-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="70133-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="70133-136">targetGroupId</span></span>|<span data-ttu-id="70133-137">String</span><span class="sxs-lookup"><span data-stu-id="70133-137">String</span></span>|<span data-ttu-id="70133-138">Identificador exclusivo de um grupo ao qual a política T&C é atribuída.</span><span class="sxs-lookup"><span data-stu-id="70133-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="70133-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="70133-139">Response</span></span>
<span data-ttu-id="70133-140">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70133-140">If successful, this method returns a `201 Created` response code and a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70133-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70133-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="70133-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70133-142">Request</span></span>
<span data-ttu-id="70133-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70133-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="70133-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="70133-144">Response</span></span>
<span data-ttu-id="70133-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70133-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





