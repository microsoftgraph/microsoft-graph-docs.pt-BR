---
title: Atualizar termsAndConditionsGroupAssignment
description: Atualize as propriedades de um objeto termsAndConditionsGroupAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ea202d33028d9eff66e06030d3049f4d6fa7aef1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393750"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="ec4b6-103">Atualizar termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="ec4b6-103">Update termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="ec4b6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ec4b6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ec4b6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ec4b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec4b6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ec4b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec4b6-107">Atualize as propriedades de um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ec4b6-107">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec4b6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ec4b6-108">Prerequisites</span></span>
<span data-ttu-id="ec4b6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ec4b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ec4b6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec4b6-111">Permission type</span></span>|<span data-ttu-id="ec4b6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ec4b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec4b6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec4b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec4b6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec4b6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ec4b6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec4b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec4b6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec4b6-116">Not supported.</span></span>|
|<span data-ttu-id="ec4b6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec4b6-117">Application</span></span>|<span data-ttu-id="ec4b6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec4b6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec4b6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec4b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ec4b6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec4b6-120">Request headers</span></span>
|<span data-ttu-id="ec4b6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec4b6-121">Header</span></span>|<span data-ttu-id="ec4b6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ec4b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec4b6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec4b6-123">Authorization</span></span>|<span data-ttu-id="ec4b6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec4b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec4b6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ec4b6-125">Accept</span></span>|<span data-ttu-id="ec4b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec4b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec4b6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec4b6-127">Request body</span></span>
<span data-ttu-id="ec4b6-128">No corpo da solicitação, fornece uma representação JSON para o objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ec4b6-128">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="ec4b6-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ec4b6-129">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="ec4b6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec4b6-130">Property</span></span>|<span data-ttu-id="ec4b6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec4b6-131">Type</span></span>|<span data-ttu-id="ec4b6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec4b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec4b6-133">id</span><span class="sxs-lookup"><span data-stu-id="ec4b6-133">id</span></span>|<span data-ttu-id="ec4b6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec4b6-134">String</span></span>|<span data-ttu-id="ec4b6-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="ec4b6-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ec4b6-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="ec4b6-136">targetGroupId</span></span>|<span data-ttu-id="ec4b6-137">String</span><span class="sxs-lookup"><span data-stu-id="ec4b6-137">String</span></span>|<span data-ttu-id="ec4b6-138">Identificador exclusivo de um grupo que a política de T&C é atribuída a.</span><span class="sxs-lookup"><span data-stu-id="ec4b6-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="ec4b6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec4b6-139">Response</span></span>
<span data-ttu-id="ec4b6-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec4b6-140">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec4b6-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec4b6-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec4b6-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec4b6-142">Request</span></span>
<span data-ttu-id="ec4b6-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec4b6-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="ec4b6-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec4b6-144">Response</span></span>
<span data-ttu-id="ec4b6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec4b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




