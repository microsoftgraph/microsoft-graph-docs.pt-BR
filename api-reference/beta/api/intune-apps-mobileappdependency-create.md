---
title: Criar mobileAppDependency
description: Criar um novo objeto mobileAppDependency.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a272a9c39262b6dd14c8d118f8c50e615d92583
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935144"
---
# <a name="create-mobileappdependency"></a><span data-ttu-id="e0253-103">Criar mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="e0253-103">Create mobileAppDependency</span></span>

> <span data-ttu-id="e0253-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e0253-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0253-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0253-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0253-106">Criar um novo objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="e0253-106">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0253-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e0253-107">Prerequisites</span></span>
<span data-ttu-id="e0253-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0253-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0253-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0253-110">Permission type</span></span>|<span data-ttu-id="e0253-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e0253-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0253-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0253-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0253-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0253-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e0253-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0253-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0253-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0253-115">Not supported.</span></span>|
|<span data-ttu-id="e0253-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0253-116">Application</span></span>|<span data-ttu-id="e0253-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0253-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0253-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0253-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="e0253-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0253-119">Request headers</span></span>
|<span data-ttu-id="e0253-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0253-120">Header</span></span>|<span data-ttu-id="e0253-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e0253-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0253-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0253-122">Authorization</span></span>|<span data-ttu-id="e0253-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0253-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0253-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e0253-124">Accept</span></span>|<span data-ttu-id="e0253-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0253-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0253-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0253-126">Request body</span></span>
<span data-ttu-id="e0253-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppDependency.</span><span class="sxs-lookup"><span data-stu-id="e0253-127">In the request body, supply a JSON representation for the mobileAppDependency object.</span></span>

<span data-ttu-id="e0253-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppDependency.</span><span class="sxs-lookup"><span data-stu-id="e0253-128">The following table shows the properties that are required when you create the mobileAppDependency.</span></span>

|<span data-ttu-id="e0253-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0253-129">Property</span></span>|<span data-ttu-id="e0253-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0253-130">Type</span></span>|<span data-ttu-id="e0253-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0253-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0253-132">id</span><span class="sxs-lookup"><span data-stu-id="e0253-132">id</span></span>|<span data-ttu-id="e0253-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0253-133">String</span></span>|<span data-ttu-id="e0253-134">A ID da entidade de relação. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="e0253-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="e0253-135">targetId</span><span class="sxs-lookup"><span data-stu-id="e0253-135">targetId</span></span>|<span data-ttu-id="e0253-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0253-136">String</span></span>|<span data-ttu-id="e0253-137">A ID de aplicativo do aplicativo móvel do filho de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="e0253-137">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="e0253-138">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="e0253-138">targetDisplayName</span></span>|<span data-ttu-id="e0253-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0253-139">String</span></span>|<span data-ttu-id="e0253-140">O nome de exibição do aplicativo móvel filho de destino.</span><span class="sxs-lookup"><span data-stu-id="e0253-140">The target child mobile app's display name.</span></span> <span data-ttu-id="e0253-141">Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="e0253-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="e0253-142">DependencyType</span><span class="sxs-lookup"><span data-stu-id="e0253-142">dependencyType</span></span>|[<span data-ttu-id="e0253-143">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="e0253-143">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="e0253-144">O tipo de relação de dependência entre os aplicativos pai e filho.</span><span class="sxs-lookup"><span data-stu-id="e0253-144">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="e0253-145">Os valores possíveis são: `detect` e `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="e0253-145">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="e0253-146">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e0253-146">dependentAppCount</span></span>|<span data-ttu-id="e0253-147">Int32</span><span class="sxs-lookup"><span data-stu-id="e0253-147">Int32</span></span>|<span data-ttu-id="e0253-148">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="e0253-148">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="e0253-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0253-149">Response</span></span>
<span data-ttu-id="e0253-150">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0253-150">If successful, this method returns a `201 Created` response code and a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0253-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0253-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0253-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0253-152">Request</span></span>
<span data-ttu-id="e0253-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0253-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```

### <a name="response"></a><span data-ttu-id="e0253-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0253-154">Response</span></span>
<span data-ttu-id="e0253-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0253-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```




