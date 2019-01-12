---
title: Criar termsAndConditionsAssignment
description: Criar um novo objeto termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 704aa0a3f86c3b65b3f2882af21010c46c02f1b9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976132"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="82057-103">Criar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="82057-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="82057-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="82057-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82057-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="82057-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82057-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="82057-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82057-107">Criar um novo objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="82057-107">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82057-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82057-108">Prerequisites</span></span>
<span data-ttu-id="82057-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82057-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82057-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82057-111">Permission type</span></span>|<span data-ttu-id="82057-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="82057-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82057-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82057-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82057-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82057-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="82057-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82057-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82057-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82057-116">Not supported.</span></span>|
|<span data-ttu-id="82057-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82057-117">Application</span></span>|<span data-ttu-id="82057-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82057-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82057-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82057-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="82057-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82057-120">Request headers</span></span>
|<span data-ttu-id="82057-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82057-121">Header</span></span>|<span data-ttu-id="82057-122">Valor</span><span class="sxs-lookup"><span data-stu-id="82057-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82057-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="82057-123">Authorization</span></span>|<span data-ttu-id="82057-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82057-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82057-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="82057-125">Accept</span></span>|<span data-ttu-id="82057-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82057-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82057-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82057-127">Request body</span></span>
<span data-ttu-id="82057-128">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditionsAssignment.</span><span class="sxs-lookup"><span data-stu-id="82057-128">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="82057-129">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditionsAssignment.</span><span class="sxs-lookup"><span data-stu-id="82057-129">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="82057-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82057-130">Property</span></span>|<span data-ttu-id="82057-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="82057-131">Type</span></span>|<span data-ttu-id="82057-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="82057-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82057-133">id</span><span class="sxs-lookup"><span data-stu-id="82057-133">id</span></span>|<span data-ttu-id="82057-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82057-134">String</span></span>|<span data-ttu-id="82057-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="82057-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="82057-136">destino</span><span class="sxs-lookup"><span data-stu-id="82057-136">target</span></span>|[<span data-ttu-id="82057-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="82057-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="82057-138">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="82057-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="82057-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="82057-139">Response</span></span>
<span data-ttu-id="82057-140">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82057-140">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82057-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82057-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="82057-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82057-142">Request</span></span>
<span data-ttu-id="82057-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82057-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82057-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="82057-144">Response</span></span>
<span data-ttu-id="82057-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82057-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





