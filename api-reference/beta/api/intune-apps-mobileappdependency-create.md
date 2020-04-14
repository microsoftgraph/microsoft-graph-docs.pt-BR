---
title: Criar mobileAppDependency
description: Criar um novo objeto mobileAppDependency.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 16931384fb343c21b4d6f8c64c19464411ecde1d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43415367"
---
# <a name="create-mobileappdependency"></a><span data-ttu-id="b1fb3-103">Criar mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="b1fb3-103">Create mobileAppDependency</span></span>

<span data-ttu-id="b1fb3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1fb3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1fb3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1fb3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1fb3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1fb3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1fb3-107">Criar um novo objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="b1fb3-107">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1fb3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b1fb3-108">Prerequisites</span></span>
<span data-ttu-id="b1fb3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1fb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1fb3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1fb3-111">Permission type</span></span>|<span data-ttu-id="b1fb3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b1fb3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1fb3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1fb3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1fb3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1fb3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b1fb3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1fb3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1fb3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1fb3-116">Not supported.</span></span>|
|<span data-ttu-id="b1fb3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1fb3-117">Application</span></span>|<span data-ttu-id="b1fb3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1fb3-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1fb3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1fb3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="b1fb3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1fb3-120">Request headers</span></span>
|<span data-ttu-id="b1fb3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1fb3-121">Header</span></span>|<span data-ttu-id="b1fb3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b1fb3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1fb3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1fb3-123">Authorization</span></span>|<span data-ttu-id="b1fb3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1fb3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1fb3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b1fb3-125">Accept</span></span>|<span data-ttu-id="b1fb3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1fb3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1fb3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1fb3-127">Request body</span></span>
<span data-ttu-id="b1fb3-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppDependency.</span><span class="sxs-lookup"><span data-stu-id="b1fb3-128">In the request body, supply a JSON representation for the mobileAppDependency object.</span></span>

<span data-ttu-id="b1fb3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppDependency.</span><span class="sxs-lookup"><span data-stu-id="b1fb3-129">The following table shows the properties that are required when you create the mobileAppDependency.</span></span>

|<span data-ttu-id="b1fb3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1fb3-130">Property</span></span>|<span data-ttu-id="b1fb3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1fb3-131">Type</span></span>|<span data-ttu-id="b1fb3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1fb3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1fb3-133">id</span><span class="sxs-lookup"><span data-stu-id="b1fb3-133">id</span></span>|<span data-ttu-id="b1fb3-134">String</span><span class="sxs-lookup"><span data-stu-id="b1fb3-134">String</span></span>|<span data-ttu-id="b1fb3-135">A ID da entidade de relação. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="b1fb3-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="b1fb3-136">targetId</span><span class="sxs-lookup"><span data-stu-id="b1fb3-136">targetId</span></span>|<span data-ttu-id="b1fb3-137">String</span><span class="sxs-lookup"><span data-stu-id="b1fb3-137">String</span></span>|<span data-ttu-id="b1fb3-138">A ID de aplicativo do aplicativo móvel do filho de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="b1fb3-138">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="b1fb3-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="b1fb3-139">targetDisplayName</span></span>|<span data-ttu-id="b1fb3-140">String</span><span class="sxs-lookup"><span data-stu-id="b1fb3-140">String</span></span>|<span data-ttu-id="b1fb3-141">O nome de exibição do aplicativo móvel filho de destino.</span><span class="sxs-lookup"><span data-stu-id="b1fb3-141">The target child mobile app's display name.</span></span> <span data-ttu-id="b1fb3-142">Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="b1fb3-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="b1fb3-143">DependencyType</span><span class="sxs-lookup"><span data-stu-id="b1fb3-143">dependencyType</span></span>|[<span data-ttu-id="b1fb3-144">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="b1fb3-144">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="b1fb3-145">O tipo de relação de dependência entre os aplicativos pai e filho.</span><span class="sxs-lookup"><span data-stu-id="b1fb3-145">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="b1fb3-146">Os valores possíveis são: `detect` e `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="b1fb3-146">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="b1fb3-147">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b1fb3-147">dependentAppCount</span></span>|<span data-ttu-id="b1fb3-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b1fb3-148">Int32</span></span>|<span data-ttu-id="b1fb3-149">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="b1fb3-149">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="b1fb3-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1fb3-150">Response</span></span>
<span data-ttu-id="b1fb3-151">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1fb3-151">If successful, this method returns a `201 Created` response code and a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1fb3-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1fb3-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1fb3-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1fb3-153">Request</span></span>
<span data-ttu-id="b1fb3-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1fb3-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b1fb3-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1fb3-155">Response</span></span>
<span data-ttu-id="b1fb3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1fb3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



