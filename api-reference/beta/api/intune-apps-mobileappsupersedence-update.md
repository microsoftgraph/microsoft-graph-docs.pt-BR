---
title: Atualizar mobileAppSupersedence
description: Atualiza as propriedades de um objeto mobileAppSupersedence.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca62f8b5ef085b526fbc5fe589c4b31a3046d6fc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992500"
---
# <a name="update-mobileappsupersedence"></a><span data-ttu-id="30527-103">Atualizar mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="30527-103">Update mobileAppSupersedence</span></span>

<span data-ttu-id="30527-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30527-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30527-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="30527-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30527-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30527-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30527-107">Atualiza as propriedades de um objeto [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) .</span><span class="sxs-lookup"><span data-stu-id="30527-107">Update the properties of a [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30527-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30527-108">Prerequisites</span></span>
<span data-ttu-id="30527-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30527-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30527-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30527-111">Permission type</span></span>|<span data-ttu-id="30527-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30527-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30527-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30527-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30527-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30527-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="30527-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30527-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30527-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30527-116">Not supported.</span></span>|
|<span data-ttu-id="30527-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30527-117">Application</span></span>|<span data-ttu-id="30527-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30527-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30527-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30527-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="30527-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30527-120">Request headers</span></span>
|<span data-ttu-id="30527-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30527-121">Header</span></span>|<span data-ttu-id="30527-122">Valor</span><span class="sxs-lookup"><span data-stu-id="30527-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30527-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="30527-123">Authorization</span></span>|<span data-ttu-id="30527-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30527-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30527-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30527-125">Accept</span></span>|<span data-ttu-id="30527-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30527-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30527-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30527-127">Request body</span></span>
<span data-ttu-id="30527-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) .</span><span class="sxs-lookup"><span data-stu-id="30527-128">In the request body, supply a JSON representation for the [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>

<span data-ttu-id="30527-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md).</span><span class="sxs-lookup"><span data-stu-id="30527-129">The following table shows the properties that are required when you create the [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md).</span></span>

|<span data-ttu-id="30527-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30527-130">Property</span></span>|<span data-ttu-id="30527-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="30527-131">Type</span></span>|<span data-ttu-id="30527-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="30527-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30527-133">id</span><span class="sxs-lookup"><span data-stu-id="30527-133">id</span></span>|<span data-ttu-id="30527-134">String</span><span class="sxs-lookup"><span data-stu-id="30527-134">String</span></span>|<span data-ttu-id="30527-135">A ID da entidade de relação. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="30527-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="30527-136">targetId</span><span class="sxs-lookup"><span data-stu-id="30527-136">targetId</span></span>|<span data-ttu-id="30527-137">String</span><span class="sxs-lookup"><span data-stu-id="30527-137">String</span></span>|<span data-ttu-id="30527-138">A ID de aplicativo do aplicativo móvel de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="30527-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="30527-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="30527-139">targetDisplayName</span></span>|<span data-ttu-id="30527-140">String</span><span class="sxs-lookup"><span data-stu-id="30527-140">String</span></span>|<span data-ttu-id="30527-141">O nome de exibição do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="30527-141">The target mobile app's display name.</span></span> <span data-ttu-id="30527-142">Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="30527-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="30527-143">targetType</span><span class="sxs-lookup"><span data-stu-id="30527-143">targetType</span></span>|[<span data-ttu-id="30527-144">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="30527-144">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="30527-145">O tipo de relação que indica se o destino é um pai ou filho.</span><span class="sxs-lookup"><span data-stu-id="30527-145">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="30527-146">Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span><span class="sxs-lookup"><span data-stu-id="30527-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="30527-147">Os valores possíveis são: `child` e `parent`.</span><span class="sxs-lookup"><span data-stu-id="30527-147">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="30527-148">supersedenceType</span><span class="sxs-lookup"><span data-stu-id="30527-148">supersedenceType</span></span>|[<span data-ttu-id="30527-149">mobileAppSupersedenceType</span><span class="sxs-lookup"><span data-stu-id="30527-149">mobileAppSupersedenceType</span></span>](../resources/intune-apps-mobileappsupersedencetype.md)|<span data-ttu-id="30527-150">O tipo de relação de substituição entre os aplicativos pai e filho.</span><span class="sxs-lookup"><span data-stu-id="30527-150">The supersedence relationship type between the parent and child apps.</span></span> <span data-ttu-id="30527-151">Os valores possíveis são: `update` e `replace`.</span><span class="sxs-lookup"><span data-stu-id="30527-151">Possible values are: `update`, `replace`.</span></span>|
|<span data-ttu-id="30527-152">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="30527-152">supersededAppCount</span></span>|<span data-ttu-id="30527-153">Int32</span><span class="sxs-lookup"><span data-stu-id="30527-153">Int32</span></span>|<span data-ttu-id="30527-154">O número total de aplicativos diretamente ou indiretamente substituídos pelo aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="30527-154">The total number of apps directly or indirectly superseded by the child app.</span></span>|
|<span data-ttu-id="30527-155">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="30527-155">supersedingAppCount</span></span>|<span data-ttu-id="30527-156">Int32</span><span class="sxs-lookup"><span data-stu-id="30527-156">Int32</span></span>|<span data-ttu-id="30527-157">O número total de aplicativos que substituem diretamente ou indiretamente o aplicativo pai.</span><span class="sxs-lookup"><span data-stu-id="30527-157">The total number of apps directly or indirectly superseding the parent app.</span></span>|



## <a name="response"></a><span data-ttu-id="30527-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="30527-158">Response</span></span>
<span data-ttu-id="30527-159">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30527-159">If successful, this method returns a `200 OK` response code and an updated [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30527-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30527-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="30527-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30527-161">Request</span></span>
<span data-ttu-id="30527-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30527-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
Content-type: application/json
Content-length: 268

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```

### <a name="response"></a><span data-ttu-id="30527-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="30527-163">Response</span></span>
<span data-ttu-id="30527-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30527-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "id": "c0254204-4204-c025-0442-25c0044225c0",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```






