---
title: Atualizar termsAndConditionsAssignment
description: Atualizar as propriedades de um objeto termsAndConditionsAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b9f689924557da084cab43eba58832a677d1dd13
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515403"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="2aef6-103">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2aef6-103">Update termsAndConditionsAssignment</span></span>

<span data-ttu-id="2aef6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2aef6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2aef6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2aef6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2aef6-106">Atualizar as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2aef6-106">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2aef6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2aef6-107">Prerequisites</span></span>
<span data-ttu-id="2aef6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2aef6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2aef6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2aef6-110">Permission type</span></span>|<span data-ttu-id="2aef6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2aef6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2aef6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2aef6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2aef6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2aef6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2aef6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2aef6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2aef6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2aef6-115">Not supported.</span></span>|
|<span data-ttu-id="2aef6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2aef6-116">Application</span></span>|<span data-ttu-id="2aef6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2aef6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2aef6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2aef6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2aef6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2aef6-119">Request headers</span></span>
|<span data-ttu-id="2aef6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2aef6-120">Header</span></span>|<span data-ttu-id="2aef6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2aef6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2aef6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2aef6-122">Authorization</span></span>|<span data-ttu-id="2aef6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2aef6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2aef6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2aef6-124">Accept</span></span>|<span data-ttu-id="2aef6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2aef6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2aef6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2aef6-126">Request body</span></span>
<span data-ttu-id="2aef6-127">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2aef6-127">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="2aef6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2aef6-128">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="2aef6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2aef6-129">Property</span></span>|<span data-ttu-id="2aef6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2aef6-130">Type</span></span>|<span data-ttu-id="2aef6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2aef6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2aef6-132">id</span><span class="sxs-lookup"><span data-stu-id="2aef6-132">id</span></span>|<span data-ttu-id="2aef6-133">String</span><span class="sxs-lookup"><span data-stu-id="2aef6-133">String</span></span>|<span data-ttu-id="2aef6-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="2aef6-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="2aef6-135">destino</span><span class="sxs-lookup"><span data-stu-id="2aef6-135">target</span></span>|[<span data-ttu-id="2aef6-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2aef6-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2aef6-137">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="2aef6-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="2aef6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2aef6-138">Response</span></span>
<span data-ttu-id="2aef6-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2aef6-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2aef6-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2aef6-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2aef6-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2aef6-141">Request</span></span>
<span data-ttu-id="2aef6-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2aef6-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="2aef6-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="2aef6-143">Response</span></span>
<span data-ttu-id="2aef6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2aef6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




