---
title: Criar targetedManagedAppConfiguration
description: Cria um novo objeto targetedManagedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6dd9b08d940bdc7167a7d9334bcf7bcb5c140468
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779038"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="4f1fc-103">Criar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4f1fc-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="4f1fc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f1fc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f1fc-106">Cria um novo objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f1fc-106">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f1fc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f1fc-107">Prerequisites</span></span>
<span data-ttu-id="4f1fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f1fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f1fc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f1fc-110">Permission type</span></span>|<span data-ttu-id="4f1fc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f1fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f1fc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f1fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f1fc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f1fc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4f1fc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f1fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f1fc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-115">Not supported.</span></span>|
|<span data-ttu-id="4f1fc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f1fc-116">Application</span></span>|<span data-ttu-id="4f1fc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f1fc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f1fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4f1fc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f1fc-119">Request headers</span></span>
|<span data-ttu-id="4f1fc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f1fc-120">Header</span></span>|<span data-ttu-id="4f1fc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4f1fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f1fc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f1fc-122">Authorization</span></span>|<span data-ttu-id="4f1fc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f1fc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f1fc-124">Accept</span></span>|<span data-ttu-id="4f1fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f1fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f1fc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f1fc-126">Request body</span></span>
<span data-ttu-id="4f1fc-127">No corpo da solicitação, forneça uma representação JSON do objeto targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-127">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="4f1fc-128">A tabela a seguir mostra as propriedades obrigatórias ao criar targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-128">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="4f1fc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f1fc-129">Property</span></span>|<span data-ttu-id="4f1fc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f1fc-130">Type</span></span>|<span data-ttu-id="4f1fc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f1fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f1fc-132">displayName</span><span class="sxs-lookup"><span data-stu-id="4f1fc-132">displayName</span></span>|<span data-ttu-id="4f1fc-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f1fc-133">String</span></span>|<span data-ttu-id="4f1fc-134">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-134">Policy display name.</span></span> <span data-ttu-id="4f1fc-135">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4f1fc-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4f1fc-136">description</span><span class="sxs-lookup"><span data-stu-id="4f1fc-136">description</span></span>|<span data-ttu-id="4f1fc-137">String</span><span class="sxs-lookup"><span data-stu-id="4f1fc-137">String</span></span>|<span data-ttu-id="4f1fc-138">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-138">The policy's description.</span></span> <span data-ttu-id="4f1fc-139">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4f1fc-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4f1fc-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f1fc-140">createdDateTime</span></span>|<span data-ttu-id="4f1fc-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f1fc-141">DateTimeOffset</span></span>|<span data-ttu-id="4f1fc-142">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-142">The date and time the policy was created.</span></span> <span data-ttu-id="4f1fc-143">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4f1fc-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4f1fc-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f1fc-144">lastModifiedDateTime</span></span>|<span data-ttu-id="4f1fc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f1fc-145">DateTimeOffset</span></span>|<span data-ttu-id="4f1fc-146">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-146">Last time the policy was modified.</span></span> <span data-ttu-id="4f1fc-147">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4f1fc-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4f1fc-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4f1fc-148">roleScopeTagIds</span></span>|<span data-ttu-id="4f1fc-149">Coleção String</span><span class="sxs-lookup"><span data-stu-id="4f1fc-149">String collection</span></span>|<span data-ttu-id="4f1fc-150">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4f1fc-151">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4f1fc-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4f1fc-152">id</span><span class="sxs-lookup"><span data-stu-id="4f1fc-152">id</span></span>|<span data-ttu-id="4f1fc-153">String</span><span class="sxs-lookup"><span data-stu-id="4f1fc-153">String</span></span>|<span data-ttu-id="4f1fc-154">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-154">Key of the entity.</span></span> <span data-ttu-id="4f1fc-155">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4f1fc-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4f1fc-156">version</span><span class="sxs-lookup"><span data-stu-id="4f1fc-156">version</span></span>|<span data-ttu-id="4f1fc-157">String</span><span class="sxs-lookup"><span data-stu-id="4f1fc-157">String</span></span>|<span data-ttu-id="4f1fc-158">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-158">Version of the entity.</span></span> <span data-ttu-id="4f1fc-159">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4f1fc-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4f1fc-160">customSettings</span><span class="sxs-lookup"><span data-stu-id="4f1fc-160">customSettings</span></span>|<span data-ttu-id="4f1fc-161">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4f1fc-161">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="4f1fc-162">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f1fc-162">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="4f1fc-163">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="4f1fc-163">deployedAppCount</span></span>|<span data-ttu-id="4f1fc-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4f1fc-164">Int32</span></span>|<span data-ttu-id="4f1fc-165">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-165">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="4f1fc-166">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4f1fc-166">isAssigned</span></span>|<span data-ttu-id="4f1fc-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f1fc-167">Boolean</span></span>|<span data-ttu-id="4f1fc-168">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-168">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="4f1fc-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f1fc-169">Response</span></span>
<span data-ttu-id="4f1fc-170">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-170">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f1fc-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f1fc-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f1fc-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f1fc-172">Request</span></span>
<span data-ttu-id="4f1fc-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
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

### <a name="response"></a><span data-ttu-id="4f1fc-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f1fc-174">Response</span></span>
<span data-ttu-id="4f1fc-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f1fc-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





