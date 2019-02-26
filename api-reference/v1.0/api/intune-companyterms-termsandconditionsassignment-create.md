---
title: Criar termsAndConditionsAssignment
description: Criar um novo objeto termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a52b60ee00f8565c9ea148c14bdfebbde309536b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257432"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="8aed3-103">Criar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="8aed3-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="8aed3-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8aed3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8aed3-105">Criar um novo objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8aed3-105">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8aed3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8aed3-106">Prerequisites</span></span>
<span data-ttu-id="8aed3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8aed3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8aed3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8aed3-109">Permission type</span></span>|<span data-ttu-id="8aed3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8aed3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8aed3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8aed3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8aed3-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aed3-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8aed3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8aed3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8aed3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8aed3-114">Not supported.</span></span>|
|<span data-ttu-id="8aed3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8aed3-115">Application</span></span>|<span data-ttu-id="8aed3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8aed3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8aed3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8aed3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8aed3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8aed3-118">Request headers</span></span>
|<span data-ttu-id="8aed3-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8aed3-119">Header</span></span>|<span data-ttu-id="8aed3-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8aed3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8aed3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8aed3-121">Authorization</span></span>|<span data-ttu-id="8aed3-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8aed3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8aed3-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8aed3-123">Accept</span></span>|<span data-ttu-id="8aed3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8aed3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8aed3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8aed3-125">Request body</span></span>
<span data-ttu-id="8aed3-126">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditionsAssignment.</span><span class="sxs-lookup"><span data-stu-id="8aed3-126">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="8aed3-127">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditionsAssignment.</span><span class="sxs-lookup"><span data-stu-id="8aed3-127">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="8aed3-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8aed3-128">Property</span></span>|<span data-ttu-id="8aed3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8aed3-129">Type</span></span>|<span data-ttu-id="8aed3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aed3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8aed3-131">id</span><span class="sxs-lookup"><span data-stu-id="8aed3-131">id</span></span>|<span data-ttu-id="8aed3-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8aed3-132">String</span></span>|<span data-ttu-id="8aed3-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="8aed3-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="8aed3-134">destino</span><span class="sxs-lookup"><span data-stu-id="8aed3-134">target</span></span>|[<span data-ttu-id="8aed3-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8aed3-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8aed3-136">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="8aed3-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="8aed3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aed3-137">Response</span></span>
<span data-ttu-id="8aed3-138">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8aed3-138">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8aed3-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8aed3-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="8aed3-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8aed3-140">Request</span></span>
<span data-ttu-id="8aed3-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8aed3-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="8aed3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aed3-142">Response</span></span>
<span data-ttu-id="8aed3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8aed3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



