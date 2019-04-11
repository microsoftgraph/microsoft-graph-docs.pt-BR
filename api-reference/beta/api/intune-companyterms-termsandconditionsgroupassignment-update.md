---
title: Atualizar termsAndConditionsGroupAssignment
description: Atualiza as propriedades de um objeto termsAndConditionsGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 650477e810035039cdc9513ac41a387539fb761c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804015"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="80a08-103">Atualizar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="80a08-103">Update termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="80a08-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="80a08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80a08-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80a08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80a08-106">Atualiza as propriedades de um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="80a08-106">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80a08-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80a08-107">Prerequisites</span></span>
<span data-ttu-id="80a08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80a08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80a08-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80a08-110">Permission type</span></span>|<span data-ttu-id="80a08-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="80a08-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80a08-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80a08-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80a08-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80a08-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="80a08-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80a08-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80a08-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80a08-115">Not supported.</span></span>|
|<span data-ttu-id="80a08-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80a08-116">Application</span></span>|<span data-ttu-id="80a08-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80a08-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80a08-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80a08-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="80a08-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80a08-119">Request headers</span></span>
|<span data-ttu-id="80a08-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80a08-120">Header</span></span>|<span data-ttu-id="80a08-121">Valor</span><span class="sxs-lookup"><span data-stu-id="80a08-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80a08-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="80a08-122">Authorization</span></span>|<span data-ttu-id="80a08-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80a08-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80a08-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="80a08-124">Accept</span></span>|<span data-ttu-id="80a08-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80a08-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80a08-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80a08-126">Request body</span></span>
<span data-ttu-id="80a08-127">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="80a08-127">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="80a08-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="80a08-128">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="80a08-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80a08-129">Property</span></span>|<span data-ttu-id="80a08-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="80a08-130">Type</span></span>|<span data-ttu-id="80a08-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="80a08-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80a08-132">id</span><span class="sxs-lookup"><span data-stu-id="80a08-132">id</span></span>|<span data-ttu-id="80a08-133">String</span><span class="sxs-lookup"><span data-stu-id="80a08-133">String</span></span>|<span data-ttu-id="80a08-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="80a08-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="80a08-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="80a08-135">targetGroupId</span></span>|<span data-ttu-id="80a08-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80a08-136">String</span></span>|<span data-ttu-id="80a08-137">Identificador exclusivo de um grupo ao qual a política T&C é atribuída.</span><span class="sxs-lookup"><span data-stu-id="80a08-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="80a08-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="80a08-138">Response</span></span>
<span data-ttu-id="80a08-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80a08-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80a08-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80a08-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="80a08-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80a08-141">Request</span></span>
<span data-ttu-id="80a08-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80a08-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="80a08-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="80a08-143">Response</span></span>
<span data-ttu-id="80a08-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80a08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





