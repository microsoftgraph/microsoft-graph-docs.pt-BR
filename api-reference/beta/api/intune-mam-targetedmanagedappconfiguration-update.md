---
title: Atualizar targetedManagedAppConfiguration
description: Atualizar as propriedades de um objeto targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22ace2319b37f664883e2021ceb5636328bb2e36
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33902945"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="4256f-103">Atualizar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4256f-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="4256f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4256f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4256f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4256f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4256f-106">Atualizar as propriedades de um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4256f-106">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4256f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4256f-107">Prerequisites</span></span>
<span data-ttu-id="4256f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4256f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4256f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4256f-110">Permission type</span></span>|<span data-ttu-id="4256f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4256f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4256f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4256f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4256f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4256f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4256f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4256f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4256f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4256f-115">Not supported.</span></span>|
|<span data-ttu-id="4256f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4256f-116">Application</span></span>|<span data-ttu-id="4256f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4256f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4256f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4256f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4256f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4256f-119">Request headers</span></span>
|<span data-ttu-id="4256f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4256f-120">Header</span></span>|<span data-ttu-id="4256f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4256f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4256f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4256f-122">Authorization</span></span>|<span data-ttu-id="4256f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4256f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4256f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4256f-124">Accept</span></span>|<span data-ttu-id="4256f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4256f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4256f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4256f-126">Request body</span></span>
<span data-ttu-id="4256f-127">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4256f-127">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="4256f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4256f-128">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="4256f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4256f-129">Property</span></span>|<span data-ttu-id="4256f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4256f-130">Type</span></span>|<span data-ttu-id="4256f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4256f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4256f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="4256f-132">displayName</span></span>|<span data-ttu-id="4256f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4256f-133">String</span></span>|<span data-ttu-id="4256f-134">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="4256f-134">Policy display name.</span></span> <span data-ttu-id="4256f-135">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4256f-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4256f-136">description</span><span class="sxs-lookup"><span data-stu-id="4256f-136">description</span></span>|<span data-ttu-id="4256f-137">String</span><span class="sxs-lookup"><span data-stu-id="4256f-137">String</span></span>|<span data-ttu-id="4256f-138">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="4256f-138">The policy's description.</span></span> <span data-ttu-id="4256f-139">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4256f-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4256f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4256f-140">createdDateTime</span></span>|<span data-ttu-id="4256f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4256f-141">DateTimeOffset</span></span>|<span data-ttu-id="4256f-142">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="4256f-142">The date and time the policy was created.</span></span> <span data-ttu-id="4256f-143">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4256f-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4256f-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4256f-144">lastModifiedDateTime</span></span>|<span data-ttu-id="4256f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4256f-145">DateTimeOffset</span></span>|<span data-ttu-id="4256f-146">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="4256f-146">Last time the policy was modified.</span></span> <span data-ttu-id="4256f-147">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4256f-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4256f-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4256f-148">roleScopeTagIds</span></span>|<span data-ttu-id="4256f-149">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4256f-149">String collection</span></span>|<span data-ttu-id="4256f-150">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="4256f-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4256f-151">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4256f-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4256f-152">id</span><span class="sxs-lookup"><span data-stu-id="4256f-152">id</span></span>|<span data-ttu-id="4256f-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4256f-153">String</span></span>|<span data-ttu-id="4256f-154">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4256f-154">Key of the entity.</span></span> <span data-ttu-id="4256f-155">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4256f-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4256f-156">version</span><span class="sxs-lookup"><span data-stu-id="4256f-156">version</span></span>|<span data-ttu-id="4256f-157">String</span><span class="sxs-lookup"><span data-stu-id="4256f-157">String</span></span>|<span data-ttu-id="4256f-158">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="4256f-158">Version of the entity.</span></span> <span data-ttu-id="4256f-159">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4256f-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4256f-160">customSettings</span><span class="sxs-lookup"><span data-stu-id="4256f-160">customSettings</span></span>|<span data-ttu-id="4256f-161">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4256f-161">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="4256f-162">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4256f-162">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="4256f-163">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="4256f-163">deployedAppCount</span></span>|<span data-ttu-id="4256f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4256f-164">Int32</span></span>|<span data-ttu-id="4256f-165">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="4256f-165">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="4256f-166">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4256f-166">isAssigned</span></span>|<span data-ttu-id="4256f-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="4256f-167">Boolean</span></span>|<span data-ttu-id="4256f-168">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="4256f-168">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="4256f-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="4256f-169">Response</span></span>
<span data-ttu-id="4256f-170">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4256f-170">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4256f-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4256f-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="4256f-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4256f-172">Request</span></span>
<span data-ttu-id="4256f-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4256f-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 450

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="4256f-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="4256f-174">Response</span></span>
<span data-ttu-id="4256f-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4256f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 622

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




