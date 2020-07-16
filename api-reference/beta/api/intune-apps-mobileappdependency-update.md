---
title: Atualizar mobileAppDependency
description: Atualiza as propriedades de um objeto mobileAppDependency.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2d1e03fc9772f4fb4d0e7833564563f6c39c399b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793301"
---
# <a name="update-mobileappdependency"></a><span data-ttu-id="efa79-103">Atualizar mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="efa79-103">Update mobileAppDependency</span></span>

<span data-ttu-id="efa79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efa79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efa79-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="efa79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efa79-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="efa79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efa79-107">Atualiza as propriedades de um objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="efa79-107">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efa79-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="efa79-108">Prerequisites</span></span>
<span data-ttu-id="efa79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efa79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efa79-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efa79-111">Permission type</span></span>|<span data-ttu-id="efa79-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="efa79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efa79-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efa79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efa79-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efa79-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="efa79-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efa79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efa79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efa79-116">Not supported.</span></span>|
|<span data-ttu-id="efa79-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efa79-117">Application</span></span>|<span data-ttu-id="efa79-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efa79-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efa79-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efa79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="efa79-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efa79-120">Request headers</span></span>
|<span data-ttu-id="efa79-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="efa79-121">Header</span></span>|<span data-ttu-id="efa79-122">Valor</span><span class="sxs-lookup"><span data-stu-id="efa79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efa79-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="efa79-123">Authorization</span></span>|<span data-ttu-id="efa79-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efa79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efa79-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="efa79-125">Accept</span></span>|<span data-ttu-id="efa79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efa79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efa79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efa79-127">Request body</span></span>
<span data-ttu-id="efa79-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="efa79-128">In the request body, supply a JSON representation for the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

<span data-ttu-id="efa79-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span><span class="sxs-lookup"><span data-stu-id="efa79-129">The following table shows the properties that are required when you create the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>

|<span data-ttu-id="efa79-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efa79-130">Property</span></span>|<span data-ttu-id="efa79-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="efa79-131">Type</span></span>|<span data-ttu-id="efa79-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="efa79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efa79-133">id</span><span class="sxs-lookup"><span data-stu-id="efa79-133">id</span></span>|<span data-ttu-id="efa79-134">String</span><span class="sxs-lookup"><span data-stu-id="efa79-134">String</span></span>|<span data-ttu-id="efa79-135">A ID da entidade de relação. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="efa79-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="efa79-136">targetId</span><span class="sxs-lookup"><span data-stu-id="efa79-136">targetId</span></span>|<span data-ttu-id="efa79-137">String</span><span class="sxs-lookup"><span data-stu-id="efa79-137">String</span></span>|<span data-ttu-id="efa79-138">A ID de aplicativo do aplicativo móvel de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="efa79-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="efa79-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="efa79-139">targetDisplayName</span></span>|<span data-ttu-id="efa79-140">String</span><span class="sxs-lookup"><span data-stu-id="efa79-140">String</span></span>|<span data-ttu-id="efa79-141">O nome de exibição do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="efa79-141">The target mobile app's display name.</span></span> <span data-ttu-id="efa79-142">Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="efa79-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="efa79-143">DependencyType</span><span class="sxs-lookup"><span data-stu-id="efa79-143">dependencyType</span></span>|[<span data-ttu-id="efa79-144">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="efa79-144">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="efa79-145">O tipo de relação de dependência entre os aplicativos pai e filho.</span><span class="sxs-lookup"><span data-stu-id="efa79-145">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="efa79-146">Os valores possíveis são: `detect` e `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="efa79-146">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="efa79-147">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="efa79-147">dependentAppCount</span></span>|<span data-ttu-id="efa79-148">Int32</span><span class="sxs-lookup"><span data-stu-id="efa79-148">Int32</span></span>|<span data-ttu-id="efa79-149">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="efa79-149">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="efa79-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="efa79-150">Response</span></span>
<span data-ttu-id="efa79-151">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efa79-151">If successful, this method returns a `200 OK` response code and an updated [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efa79-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efa79-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="efa79-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efa79-153">Request</span></span>
<span data-ttu-id="efa79-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efa79-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
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

### <a name="response"></a><span data-ttu-id="efa79-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="efa79-155">Response</span></span>
<span data-ttu-id="efa79-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efa79-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



