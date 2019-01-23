---
title: Atualizar termsAndConditionsAssignment
description: Atualizar as propriedades de um objeto termsAndConditionsAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 67a6c83003fdc47291c91daedbc49c94cf4b16ec
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424837"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="29c42-103">Atualizar termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="29c42-103">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="29c42-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="29c42-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="29c42-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="29c42-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29c42-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="29c42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29c42-107">Atualizar as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="29c42-107">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29c42-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29c42-108">Prerequisites</span></span>
<span data-ttu-id="29c42-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="29c42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="29c42-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29c42-111">Permission type</span></span>|<span data-ttu-id="29c42-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29c42-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29c42-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29c42-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29c42-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29c42-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="29c42-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29c42-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29c42-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29c42-116">Not supported.</span></span>|
|<span data-ttu-id="29c42-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29c42-117">Application</span></span>|<span data-ttu-id="29c42-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29c42-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29c42-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29c42-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="29c42-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29c42-120">Request headers</span></span>
|<span data-ttu-id="29c42-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29c42-121">Header</span></span>|<span data-ttu-id="29c42-122">Valor</span><span class="sxs-lookup"><span data-stu-id="29c42-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29c42-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="29c42-123">Authorization</span></span>|<span data-ttu-id="29c42-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29c42-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29c42-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29c42-125">Accept</span></span>|<span data-ttu-id="29c42-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29c42-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29c42-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29c42-127">Request body</span></span>
<span data-ttu-id="29c42-128">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="29c42-128">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="29c42-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="29c42-129">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="29c42-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29c42-130">Property</span></span>|<span data-ttu-id="29c42-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="29c42-131">Type</span></span>|<span data-ttu-id="29c42-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="29c42-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29c42-133">id</span><span class="sxs-lookup"><span data-stu-id="29c42-133">id</span></span>|<span data-ttu-id="29c42-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29c42-134">String</span></span>|<span data-ttu-id="29c42-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="29c42-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="29c42-136">destino</span><span class="sxs-lookup"><span data-stu-id="29c42-136">target</span></span>|[<span data-ttu-id="29c42-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="29c42-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="29c42-138">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="29c42-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="29c42-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="29c42-139">Response</span></span>
<span data-ttu-id="29c42-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29c42-140">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29c42-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29c42-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="29c42-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29c42-142">Request</span></span>
<span data-ttu-id="29c42-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29c42-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="29c42-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="29c42-144">Response</span></span>
<span data-ttu-id="29c42-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29c42-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




