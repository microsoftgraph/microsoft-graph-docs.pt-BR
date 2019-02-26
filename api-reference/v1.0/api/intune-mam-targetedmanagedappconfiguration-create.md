---
title: Criar targetedManagedAppConfiguration
description: Cria um novo objeto targetedManagedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bde6402cb0cc17e3167b7b0e7b27568eb228c014
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251395"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="3c455-103">Criar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="3c455-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="3c455-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c455-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c455-105">Cria um novo objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c455-105">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c455-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c455-106">Prerequisites</span></span>
<span data-ttu-id="3c455-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3c455-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3c455-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c455-109">Permission type</span></span>|<span data-ttu-id="3c455-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c455-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c455-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c455-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3c455-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c455-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3c455-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c455-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c455-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c455-114">Not supported.</span></span>|
|<span data-ttu-id="3c455-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c455-115">Application</span></span>|<span data-ttu-id="3c455-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c455-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c455-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c455-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3c455-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c455-118">Request headers</span></span>
|<span data-ttu-id="3c455-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c455-119">Header</span></span>|<span data-ttu-id="3c455-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3c455-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c455-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c455-121">Authorization</span></span>|<span data-ttu-id="3c455-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c455-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c455-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c455-123">Accept</span></span>|<span data-ttu-id="3c455-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3c455-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c455-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c455-125">Request body</span></span>
<span data-ttu-id="3c455-126">No corpo da solicitação, forneça uma representação JSON do objeto targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3c455-126">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="3c455-127">A tabela a seguir mostra as propriedades obrigatórias ao criar targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3c455-127">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="3c455-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c455-128">Property</span></span>|<span data-ttu-id="3c455-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c455-129">Type</span></span>|<span data-ttu-id="3c455-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c455-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c455-131">displayName</span><span class="sxs-lookup"><span data-stu-id="3c455-131">displayName</span></span>|<span data-ttu-id="3c455-132">String</span><span class="sxs-lookup"><span data-stu-id="3c455-132">String</span></span>|<span data-ttu-id="3c455-133">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="3c455-133">Policy display name.</span></span> <span data-ttu-id="3c455-134">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3c455-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3c455-135">descrição</span><span class="sxs-lookup"><span data-stu-id="3c455-135">description</span></span>|<span data-ttu-id="3c455-136">String</span><span class="sxs-lookup"><span data-stu-id="3c455-136">String</span></span>|<span data-ttu-id="3c455-137">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="3c455-137">The policy's description.</span></span> <span data-ttu-id="3c455-138">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3c455-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3c455-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c455-139">createdDateTime</span></span>|<span data-ttu-id="3c455-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c455-140">DateTimeOffset</span></span>|<span data-ttu-id="3c455-141">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="3c455-141">The date and time the policy was created.</span></span> <span data-ttu-id="3c455-142">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3c455-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3c455-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c455-143">lastModifiedDateTime</span></span>|<span data-ttu-id="3c455-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c455-144">DateTimeOffset</span></span>|<span data-ttu-id="3c455-145">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="3c455-145">Last time the policy was modified.</span></span> <span data-ttu-id="3c455-146">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3c455-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3c455-147">id</span><span class="sxs-lookup"><span data-stu-id="3c455-147">id</span></span>|<span data-ttu-id="3c455-148">String</span><span class="sxs-lookup"><span data-stu-id="3c455-148">String</span></span>|<span data-ttu-id="3c455-149">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3c455-149">Key of the entity.</span></span> <span data-ttu-id="3c455-150">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3c455-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3c455-151">version</span><span class="sxs-lookup"><span data-stu-id="3c455-151">version</span></span>|<span data-ttu-id="3c455-152">String</span><span class="sxs-lookup"><span data-stu-id="3c455-152">String</span></span>|<span data-ttu-id="3c455-153">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="3c455-153">Version of the entity.</span></span> <span data-ttu-id="3c455-154">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3c455-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3c455-155">customSettings</span><span class="sxs-lookup"><span data-stu-id="3c455-155">customSettings</span></span>|<span data-ttu-id="3c455-156">Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="3c455-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3c455-157">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c455-157">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="3c455-158">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="3c455-158">deployedAppCount</span></span>|<span data-ttu-id="3c455-159">Int32</span><span class="sxs-lookup"><span data-stu-id="3c455-159">Int32</span></span>|<span data-ttu-id="3c455-160">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="3c455-160">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="3c455-161">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3c455-161">isAssigned</span></span>|<span data-ttu-id="3c455-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c455-162">Boolean</span></span>|<span data-ttu-id="3c455-163">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="3c455-163">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="3c455-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c455-164">Response</span></span>
<span data-ttu-id="3c455-165">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c455-165">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c455-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c455-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c455-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c455-167">Request</span></span>
<span data-ttu-id="3c455-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c455-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 388

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="3c455-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c455-169">Response</span></span>
<span data-ttu-id="3c455-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c455-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "2444e029-e029-2444-29e0-442429e04424",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```



