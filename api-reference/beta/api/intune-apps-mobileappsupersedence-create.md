---
title: Criar mobileAppSupersedence
description: Criar um novo objeto mobileAppSupersedence.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b3e5259c68a10168f4fa7c0d05714956d922e52f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247983"
---
# <a name="create-mobileappsupersedence"></a><span data-ttu-id="66e22-103">Criar mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="66e22-103">Create mobileAppSupersedence</span></span>

<span data-ttu-id="66e22-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66e22-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66e22-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="66e22-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66e22-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="66e22-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66e22-107">Criar um novo objeto [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) .</span><span class="sxs-lookup"><span data-stu-id="66e22-107">Create a new [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66e22-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="66e22-108">Prerequisites</span></span>
<span data-ttu-id="66e22-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66e22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66e22-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66e22-111">Permission type</span></span>|<span data-ttu-id="66e22-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="66e22-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66e22-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66e22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66e22-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66e22-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66e22-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66e22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66e22-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66e22-116">Not supported.</span></span>|
|<span data-ttu-id="66e22-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66e22-117">Application</span></span>|<span data-ttu-id="66e22-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66e22-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66e22-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66e22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="66e22-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66e22-120">Request headers</span></span>
|<span data-ttu-id="66e22-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="66e22-121">Header</span></span>|<span data-ttu-id="66e22-122">Valor</span><span class="sxs-lookup"><span data-stu-id="66e22-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66e22-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="66e22-123">Authorization</span></span>|<span data-ttu-id="66e22-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66e22-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66e22-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="66e22-125">Accept</span></span>|<span data-ttu-id="66e22-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66e22-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66e22-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66e22-127">Request body</span></span>
<span data-ttu-id="66e22-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppSupersedence.</span><span class="sxs-lookup"><span data-stu-id="66e22-128">In the request body, supply a JSON representation for the mobileAppSupersedence object.</span></span>

<span data-ttu-id="66e22-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppSupersedence.</span><span class="sxs-lookup"><span data-stu-id="66e22-129">The following table shows the properties that are required when you create the mobileAppSupersedence.</span></span>

|<span data-ttu-id="66e22-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66e22-130">Property</span></span>|<span data-ttu-id="66e22-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="66e22-131">Type</span></span>|<span data-ttu-id="66e22-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="66e22-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66e22-133">id</span><span class="sxs-lookup"><span data-stu-id="66e22-133">id</span></span>|<span data-ttu-id="66e22-134">String</span><span class="sxs-lookup"><span data-stu-id="66e22-134">String</span></span>|<span data-ttu-id="66e22-135">A ID da entidade de relação. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="66e22-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="66e22-136">targetId</span><span class="sxs-lookup"><span data-stu-id="66e22-136">targetId</span></span>|<span data-ttu-id="66e22-137">String</span><span class="sxs-lookup"><span data-stu-id="66e22-137">String</span></span>|<span data-ttu-id="66e22-138">A ID de aplicativo do aplicativo móvel de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="66e22-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="66e22-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="66e22-139">targetDisplayName</span></span>|<span data-ttu-id="66e22-140">String</span><span class="sxs-lookup"><span data-stu-id="66e22-140">String</span></span>|<span data-ttu-id="66e22-141">O nome de exibição do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="66e22-141">The target mobile app's display name.</span></span> <span data-ttu-id="66e22-142">Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="66e22-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="66e22-143">targetDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="66e22-143">targetDisplayVersion</span></span>|<span data-ttu-id="66e22-144">String</span><span class="sxs-lookup"><span data-stu-id="66e22-144">String</span></span>|<span data-ttu-id="66e22-145">A versão de exibição do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="66e22-145">The target mobile app's display version.</span></span> <span data-ttu-id="66e22-146">Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="66e22-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="66e22-147">targetPublisher</span><span class="sxs-lookup"><span data-stu-id="66e22-147">targetPublisher</span></span>|<span data-ttu-id="66e22-148">String</span><span class="sxs-lookup"><span data-stu-id="66e22-148">String</span></span>|<span data-ttu-id="66e22-149">O fornecedor do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="66e22-149">The target mobile app's publisher.</span></span> <span data-ttu-id="66e22-150">Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="66e22-150">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="66e22-151">targetType</span><span class="sxs-lookup"><span data-stu-id="66e22-151">targetType</span></span>|[<span data-ttu-id="66e22-152">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="66e22-152">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="66e22-153">O tipo de relação que indica se o destino é um pai ou filho.</span><span class="sxs-lookup"><span data-stu-id="66e22-153">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="66e22-154">Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span><span class="sxs-lookup"><span data-stu-id="66e22-154">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="66e22-155">Os valores possíveis são: `child` e `parent`.</span><span class="sxs-lookup"><span data-stu-id="66e22-155">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="66e22-156">supersedenceType</span><span class="sxs-lookup"><span data-stu-id="66e22-156">supersedenceType</span></span>|[<span data-ttu-id="66e22-157">mobileAppSupersedenceType</span><span class="sxs-lookup"><span data-stu-id="66e22-157">mobileAppSupersedenceType</span></span>](../resources/intune-apps-mobileappsupersedencetype.md)|<span data-ttu-id="66e22-158">O tipo de relação de substituição entre os aplicativos pai e filho.</span><span class="sxs-lookup"><span data-stu-id="66e22-158">The supersedence relationship type between the parent and child apps.</span></span> <span data-ttu-id="66e22-159">Os valores possíveis são: `update` e `replace`.</span><span class="sxs-lookup"><span data-stu-id="66e22-159">Possible values are: `update`, `replace`.</span></span>|
|<span data-ttu-id="66e22-160">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="66e22-160">supersededAppCount</span></span>|<span data-ttu-id="66e22-161">Int32</span><span class="sxs-lookup"><span data-stu-id="66e22-161">Int32</span></span>|<span data-ttu-id="66e22-162">O número total de aplicativos diretamente ou indiretamente substituídos pelo aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="66e22-162">The total number of apps directly or indirectly superseded by the child app.</span></span>|
|<span data-ttu-id="66e22-163">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="66e22-163">supersedingAppCount</span></span>|<span data-ttu-id="66e22-164">Int32</span><span class="sxs-lookup"><span data-stu-id="66e22-164">Int32</span></span>|<span data-ttu-id="66e22-165">O número total de aplicativos que substituem diretamente ou indiretamente o aplicativo pai.</span><span class="sxs-lookup"><span data-stu-id="66e22-165">The total number of apps directly or indirectly superseding the parent app.</span></span>|



## <a name="response"></a><span data-ttu-id="66e22-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="66e22-166">Response</span></span>
<span data-ttu-id="66e22-167">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66e22-167">If successful, this method returns a `201 Created` response code and a [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66e22-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66e22-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="66e22-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66e22-169">Request</span></span>
<span data-ttu-id="66e22-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66e22-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```

### <a name="response"></a><span data-ttu-id="66e22-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="66e22-171">Response</span></span>
<span data-ttu-id="66e22-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66e22-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 424

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "id": "c0254204-4204-c025-0442-25c0044225c0",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```




