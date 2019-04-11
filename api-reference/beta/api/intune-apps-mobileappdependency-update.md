---
title: Atualizar mobileAppDependency
description: Atualiza as propriedades de um objeto mobileAppDependency.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8648fb92953ef8ece7be672e746bffbb63393859
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31808859"
---
# <a name="update-mobileappdependency"></a><span data-ttu-id="942fb-103">Atualizar mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="942fb-103">Update mobileAppDependency</span></span>

> <span data-ttu-id="942fb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="942fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="942fb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="942fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="942fb-106">Atualiza as propriedades de um objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="942fb-106">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="942fb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="942fb-107">Prerequisites</span></span>
<span data-ttu-id="942fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="942fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="942fb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="942fb-110">Permission type</span></span>|<span data-ttu-id="942fb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="942fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="942fb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="942fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="942fb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="942fb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="942fb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="942fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="942fb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="942fb-115">Not supported.</span></span>|
|<span data-ttu-id="942fb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="942fb-116">Application</span></span>|<span data-ttu-id="942fb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="942fb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="942fb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="942fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="942fb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="942fb-119">Request headers</span></span>
|<span data-ttu-id="942fb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="942fb-120">Header</span></span>|<span data-ttu-id="942fb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="942fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="942fb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="942fb-122">Authorization</span></span>|<span data-ttu-id="942fb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="942fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="942fb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="942fb-124">Accept</span></span>|<span data-ttu-id="942fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="942fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="942fb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="942fb-126">Request body</span></span>
<span data-ttu-id="942fb-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="942fb-127">In the request body, supply a JSON representation for the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

<span data-ttu-id="942fb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span><span class="sxs-lookup"><span data-stu-id="942fb-128">The following table shows the properties that are required when you create the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>

|<span data-ttu-id="942fb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="942fb-129">Property</span></span>|<span data-ttu-id="942fb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="942fb-130">Type</span></span>|<span data-ttu-id="942fb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="942fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="942fb-132">id</span><span class="sxs-lookup"><span data-stu-id="942fb-132">id</span></span>|<span data-ttu-id="942fb-133">String</span><span class="sxs-lookup"><span data-stu-id="942fb-133">String</span></span>|<span data-ttu-id="942fb-134">A ID da entidade de relação. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="942fb-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="942fb-135">targetId</span><span class="sxs-lookup"><span data-stu-id="942fb-135">targetId</span></span>|<span data-ttu-id="942fb-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="942fb-136">String</span></span>|<span data-ttu-id="942fb-137">A ID de aplicativo do aplicativo móvel do filho de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="942fb-137">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="942fb-138">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="942fb-138">targetDisplayName</span></span>|<span data-ttu-id="942fb-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="942fb-139">String</span></span>|<span data-ttu-id="942fb-140">O nome de exibição do aplicativo móvel filho de destino.</span><span class="sxs-lookup"><span data-stu-id="942fb-140">The target child mobile app's display name.</span></span> <span data-ttu-id="942fb-141">Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="942fb-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="942fb-142">DependencyType</span><span class="sxs-lookup"><span data-stu-id="942fb-142">dependencyType</span></span>|[<span data-ttu-id="942fb-143">mobileAppDependecyType</span><span class="sxs-lookup"><span data-stu-id="942fb-143">mobileAppDependecyType</span></span>](../resources/intune-apps-mobileappdependecytype.md)|<span data-ttu-id="942fb-144">O tipo de relação de dependência entre os aplicativos pai e filho.</span><span class="sxs-lookup"><span data-stu-id="942fb-144">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="942fb-145">Os valores possíveis são: `detect` e `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="942fb-145">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="942fb-146">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="942fb-146">dependentAppCount</span></span>|<span data-ttu-id="942fb-147">Int32</span><span class="sxs-lookup"><span data-stu-id="942fb-147">Int32</span></span>|<span data-ttu-id="942fb-148">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="942fb-148">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="942fb-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="942fb-149">Response</span></span>
<span data-ttu-id="942fb-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="942fb-150">If successful, this method returns a `200 OK` response code and an updated [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="942fb-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="942fb-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="942fb-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="942fb-152">Request</span></span>
<span data-ttu-id="942fb-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="942fb-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="942fb-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="942fb-154">Response</span></span>
<span data-ttu-id="942fb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="942fb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





