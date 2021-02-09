---
title: Atualizar mobileAppDependency
description: Atualizar as propriedades de um objeto mobileAppDependency.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 45bb4504fc2d65a7d9284e15e73d6c5da575f881
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155311"
---
# <a name="update-mobileappdependency"></a><span data-ttu-id="d8bd8-103">Atualizar mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d8bd8-103">Update mobileAppDependency</span></span>

<span data-ttu-id="d8bd8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8bd8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8bd8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8bd8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8bd8-107">Atualizar as propriedades de um [objeto mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)</span><span class="sxs-lookup"><span data-stu-id="d8bd8-107">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8bd8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8bd8-108">Prerequisites</span></span>
<span data-ttu-id="d8bd8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8bd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8bd8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8bd8-111">Permission type</span></span>|<span data-ttu-id="d8bd8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8bd8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8bd8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8bd8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8bd8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8bd8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d8bd8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8bd8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8bd8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-116">Not supported.</span></span>|
|<span data-ttu-id="d8bd8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8bd8-117">Application</span></span>|<span data-ttu-id="d8bd8-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8bd8-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8bd8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8bd8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="d8bd8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8bd8-120">Request headers</span></span>
|<span data-ttu-id="d8bd8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8bd8-121">Header</span></span>|<span data-ttu-id="d8bd8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d8bd8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8bd8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8bd8-123">Authorization</span></span>|<span data-ttu-id="d8bd8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8bd8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8bd8-125">Accept</span></span>|<span data-ttu-id="d8bd8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8bd8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8bd8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8bd8-127">Request body</span></span>
<span data-ttu-id="d8bd8-128">No corpo da solicitação, fornece uma representação JSON do [objeto mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)</span><span class="sxs-lookup"><span data-stu-id="d8bd8-128">In the request body, supply a JSON representation for the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

<span data-ttu-id="d8bd8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span><span class="sxs-lookup"><span data-stu-id="d8bd8-129">The following table shows the properties that are required when you create the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>

|<span data-ttu-id="d8bd8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8bd8-130">Property</span></span>|<span data-ttu-id="d8bd8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8bd8-131">Type</span></span>|<span data-ttu-id="d8bd8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8bd8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8bd8-133">id</span><span class="sxs-lookup"><span data-stu-id="d8bd8-133">id</span></span>|<span data-ttu-id="d8bd8-134">String</span><span class="sxs-lookup"><span data-stu-id="d8bd8-134">String</span></span>|<span data-ttu-id="d8bd8-135">A ID da entidade de relação. Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d8bd8-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d8bd8-136">targetId</span><span class="sxs-lookup"><span data-stu-id="d8bd8-136">targetId</span></span>|<span data-ttu-id="d8bd8-137">String</span><span class="sxs-lookup"><span data-stu-id="d8bd8-137">String</span></span>|<span data-ttu-id="d8bd8-138">A ID do aplicativo móvel de destino. Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d8bd8-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d8bd8-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="d8bd8-139">targetDisplayName</span></span>|<span data-ttu-id="d8bd8-140">String</span><span class="sxs-lookup"><span data-stu-id="d8bd8-140">String</span></span>|<span data-ttu-id="d8bd8-141">O nome de exibição do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-141">The target mobile app's display name.</span></span> <span data-ttu-id="d8bd8-142">Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d8bd8-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d8bd8-143">targetDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="d8bd8-143">targetDisplayVersion</span></span>|<span data-ttu-id="d8bd8-144">String</span><span class="sxs-lookup"><span data-stu-id="d8bd8-144">String</span></span>|<span data-ttu-id="d8bd8-145">A versão de exibição do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-145">The target mobile app's display version.</span></span> <span data-ttu-id="d8bd8-146">Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d8bd8-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d8bd8-147">targetPublisher</span><span class="sxs-lookup"><span data-stu-id="d8bd8-147">targetPublisher</span></span>|<span data-ttu-id="d8bd8-148">String</span><span class="sxs-lookup"><span data-stu-id="d8bd8-148">String</span></span>|<span data-ttu-id="d8bd8-149">O editor do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-149">The target mobile app's publisher.</span></span> <span data-ttu-id="d8bd8-150">Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d8bd8-150">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d8bd8-151">targetType</span><span class="sxs-lookup"><span data-stu-id="d8bd8-151">targetType</span></span>|[<span data-ttu-id="d8bd8-152">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="d8bd8-152">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="d8bd8-153">O tipo de relação que indica se o destino é um pai ou filho.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-153">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="d8bd8-154">Herdado [de mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span><span class="sxs-lookup"><span data-stu-id="d8bd8-154">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="d8bd8-155">Os valores possíveis são: `child` e `parent`.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-155">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="d8bd8-156">dependencyType</span><span class="sxs-lookup"><span data-stu-id="d8bd8-156">dependencyType</span></span>|[<span data-ttu-id="d8bd8-157">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="d8bd8-157">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="d8bd8-158">O tipo de relação de dependência entre os aplicativos pai e filho.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-158">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="d8bd8-159">Os valores possíveis são: `detect` e `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-159">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="d8bd8-160">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="d8bd8-160">dependentAppCount</span></span>|<span data-ttu-id="d8bd8-161">Int32</span><span class="sxs-lookup"><span data-stu-id="d8bd8-161">Int32</span></span>|<span data-ttu-id="d8bd8-162">O número total de aplicativos que dependem direta ou indiretamente do aplicativo pai.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-162">The total number of apps that directly or indirectly depend on the parent app.</span></span>|
|<span data-ttu-id="d8bd8-163">dependsOnAppCount</span><span class="sxs-lookup"><span data-stu-id="d8bd8-163">dependsOnAppCount</span></span>|<span data-ttu-id="d8bd8-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d8bd8-164">Int32</span></span>|<span data-ttu-id="d8bd8-165">O número total de aplicativos dos quais o aplicativo filho está direta ou indiretamente depende.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-165">The total number of apps the child app directly or indirectly depends on.</span></span>|



## <a name="response"></a><span data-ttu-id="d8bd8-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8bd8-166">Response</span></span>
<span data-ttu-id="d8bd8-167">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8bd8-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8bd8-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8bd8-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8bd8-169">Request</span></span>
<span data-ttu-id="d8bd8-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
Content-type: application/json
Content-length: 372

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1,
  "dependsOnAppCount": 1
}
```

### <a name="response"></a><span data-ttu-id="d8bd8-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8bd8-171">Response</span></span>
<span data-ttu-id="d8bd8-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 421

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1,
  "dependsOnAppCount": 1
}
```




