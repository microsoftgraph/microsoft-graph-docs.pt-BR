---
title: Criar mobileAppDependency
description: Criar um novo objeto mobileAppDependency.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc7fa701835678deb9256b36f0aa9fe9dceb75a6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49248585"
---
# <a name="create-mobileappdependency"></a><span data-ttu-id="c8944-103">Criar mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="c8944-103">Create mobileAppDependency</span></span>

<span data-ttu-id="c8944-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8944-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8944-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8944-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8944-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8944-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8944-107">Criar um novo objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="c8944-107">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8944-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8944-108">Prerequisites</span></span>
<span data-ttu-id="c8944-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8944-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8944-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8944-111">Permission type</span></span>|<span data-ttu-id="c8944-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c8944-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8944-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8944-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8944-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8944-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c8944-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8944-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8944-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8944-116">Not supported.</span></span>|
|<span data-ttu-id="c8944-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8944-117">Application</span></span>|<span data-ttu-id="c8944-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8944-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8944-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8944-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="c8944-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8944-120">Request headers</span></span>
|<span data-ttu-id="c8944-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8944-121">Header</span></span>|<span data-ttu-id="c8944-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c8944-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8944-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8944-123">Authorization</span></span>|<span data-ttu-id="c8944-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8944-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8944-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8944-125">Accept</span></span>|<span data-ttu-id="c8944-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8944-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8944-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8944-127">Request body</span></span>
<span data-ttu-id="c8944-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppDependency.</span><span class="sxs-lookup"><span data-stu-id="c8944-128">In the request body, supply a JSON representation for the mobileAppDependency object.</span></span>

<span data-ttu-id="c8944-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppDependency.</span><span class="sxs-lookup"><span data-stu-id="c8944-129">The following table shows the properties that are required when you create the mobileAppDependency.</span></span>

|<span data-ttu-id="c8944-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8944-130">Property</span></span>|<span data-ttu-id="c8944-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8944-131">Type</span></span>|<span data-ttu-id="c8944-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8944-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8944-133">id</span><span class="sxs-lookup"><span data-stu-id="c8944-133">id</span></span>|<span data-ttu-id="c8944-134">String</span><span class="sxs-lookup"><span data-stu-id="c8944-134">String</span></span>|<span data-ttu-id="c8944-135">A ID da entidade de relação. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="c8944-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="c8944-136">targetId</span><span class="sxs-lookup"><span data-stu-id="c8944-136">targetId</span></span>|<span data-ttu-id="c8944-137">String</span><span class="sxs-lookup"><span data-stu-id="c8944-137">String</span></span>|<span data-ttu-id="c8944-138">A ID de aplicativo do aplicativo móvel de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="c8944-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="c8944-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="c8944-139">targetDisplayName</span></span>|<span data-ttu-id="c8944-140">String</span><span class="sxs-lookup"><span data-stu-id="c8944-140">String</span></span>|<span data-ttu-id="c8944-141">O nome de exibição do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="c8944-141">The target mobile app's display name.</span></span> <span data-ttu-id="c8944-142">Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="c8944-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="c8944-143">targetDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="c8944-143">targetDisplayVersion</span></span>|<span data-ttu-id="c8944-144">String</span><span class="sxs-lookup"><span data-stu-id="c8944-144">String</span></span>|<span data-ttu-id="c8944-145">A versão de exibição do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="c8944-145">The target mobile app's display version.</span></span> <span data-ttu-id="c8944-146">Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="c8944-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="c8944-147">targetPublisher</span><span class="sxs-lookup"><span data-stu-id="c8944-147">targetPublisher</span></span>|<span data-ttu-id="c8944-148">String</span><span class="sxs-lookup"><span data-stu-id="c8944-148">String</span></span>|<span data-ttu-id="c8944-149">O fornecedor do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="c8944-149">The target mobile app's publisher.</span></span> <span data-ttu-id="c8944-150">Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="c8944-150">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="c8944-151">targetType</span><span class="sxs-lookup"><span data-stu-id="c8944-151">targetType</span></span>|[<span data-ttu-id="c8944-152">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="c8944-152">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="c8944-153">O tipo de relação que indica se o destino é um pai ou filho.</span><span class="sxs-lookup"><span data-stu-id="c8944-153">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="c8944-154">Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span><span class="sxs-lookup"><span data-stu-id="c8944-154">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="c8944-155">Os valores possíveis são: `child` e `parent`.</span><span class="sxs-lookup"><span data-stu-id="c8944-155">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="c8944-156">DependencyType</span><span class="sxs-lookup"><span data-stu-id="c8944-156">dependencyType</span></span>|[<span data-ttu-id="c8944-157">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="c8944-157">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="c8944-158">O tipo de relação de dependência entre os aplicativos pai e filho.</span><span class="sxs-lookup"><span data-stu-id="c8944-158">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="c8944-159">Os valores possíveis são: `detect` e `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="c8944-159">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="c8944-160">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="c8944-160">dependentAppCount</span></span>|<span data-ttu-id="c8944-161">Int32</span><span class="sxs-lookup"><span data-stu-id="c8944-161">Int32</span></span>|<span data-ttu-id="c8944-162">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="c8944-162">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="c8944-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8944-163">Response</span></span>
<span data-ttu-id="c8944-164">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8944-164">If successful, this method returns a `201 Created` response code and a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8944-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8944-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8944-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8944-166">Request</span></span>
<span data-ttu-id="c8944-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8944-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
Content-type: application/json
Content-length: 345

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```

### <a name="response"></a><span data-ttu-id="c8944-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8944-168">Response</span></span>
<span data-ttu-id="c8944-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8944-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```




