---
title: Atualizar targetedManagedAppConfiguration
description: Atualizar as propriedades de um objeto targetedManagedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6be14c8c01a2253754e9448789e705812426f662
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783609"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="d9659-103">Atualizar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9659-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="d9659-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9659-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9659-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9659-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9659-106">Atualizar as propriedades de um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9659-106">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9659-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9659-107">Prerequisites</span></span>
<span data-ttu-id="d9659-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9659-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9659-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9659-110">Permission type</span></span>|<span data-ttu-id="d9659-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9659-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9659-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9659-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9659-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9659-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d9659-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9659-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9659-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9659-115">Not supported.</span></span>|
|<span data-ttu-id="d9659-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9659-116">Application</span></span>|<span data-ttu-id="d9659-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9659-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9659-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9659-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d9659-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9659-119">Request headers</span></span>
|<span data-ttu-id="d9659-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9659-120">Header</span></span>|<span data-ttu-id="d9659-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d9659-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9659-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9659-122">Authorization</span></span>|<span data-ttu-id="d9659-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9659-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9659-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9659-124">Accept</span></span>|<span data-ttu-id="d9659-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d9659-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9659-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9659-126">Request body</span></span>
<span data-ttu-id="d9659-127">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9659-127">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="d9659-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9659-128">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="d9659-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9659-129">Property</span></span>|<span data-ttu-id="d9659-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9659-130">Type</span></span>|<span data-ttu-id="d9659-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9659-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9659-132">displayName</span><span class="sxs-lookup"><span data-stu-id="d9659-132">displayName</span></span>|<span data-ttu-id="d9659-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9659-133">String</span></span>|<span data-ttu-id="d9659-134">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="d9659-134">Policy display name.</span></span> <span data-ttu-id="d9659-135">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d9659-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9659-136">description</span><span class="sxs-lookup"><span data-stu-id="d9659-136">description</span></span>|<span data-ttu-id="d9659-137">String</span><span class="sxs-lookup"><span data-stu-id="d9659-137">String</span></span>|<span data-ttu-id="d9659-138">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="d9659-138">The policy's description.</span></span> <span data-ttu-id="d9659-139">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d9659-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9659-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9659-140">createdDateTime</span></span>|<span data-ttu-id="d9659-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9659-141">DateTimeOffset</span></span>|<span data-ttu-id="d9659-142">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="d9659-142">The date and time the policy was created.</span></span> <span data-ttu-id="d9659-143">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d9659-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9659-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9659-144">lastModifiedDateTime</span></span>|<span data-ttu-id="d9659-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9659-145">DateTimeOffset</span></span>|<span data-ttu-id="d9659-146">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="d9659-146">Last time the policy was modified.</span></span> <span data-ttu-id="d9659-147">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d9659-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9659-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d9659-148">roleScopeTagIds</span></span>|<span data-ttu-id="d9659-149">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d9659-149">String collection</span></span>|<span data-ttu-id="d9659-150">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d9659-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d9659-151">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d9659-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9659-152">id</span><span class="sxs-lookup"><span data-stu-id="d9659-152">id</span></span>|<span data-ttu-id="d9659-153">String</span><span class="sxs-lookup"><span data-stu-id="d9659-153">String</span></span>|<span data-ttu-id="d9659-154">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d9659-154">Key of the entity.</span></span> <span data-ttu-id="d9659-155">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d9659-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9659-156">version</span><span class="sxs-lookup"><span data-stu-id="d9659-156">version</span></span>|<span data-ttu-id="d9659-157">String</span><span class="sxs-lookup"><span data-stu-id="d9659-157">String</span></span>|<span data-ttu-id="d9659-158">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="d9659-158">Version of the entity.</span></span> <span data-ttu-id="d9659-159">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d9659-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9659-160">customSettings</span><span class="sxs-lookup"><span data-stu-id="d9659-160">customSettings</span></span>|<span data-ttu-id="d9659-161">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d9659-161">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d9659-162">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9659-162">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="d9659-163">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="d9659-163">deployedAppCount</span></span>|<span data-ttu-id="d9659-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d9659-164">Int32</span></span>|<span data-ttu-id="d9659-165">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="d9659-165">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="d9659-166">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d9659-166">isAssigned</span></span>|<span data-ttu-id="d9659-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9659-167">Boolean</span></span>|<span data-ttu-id="d9659-168">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="d9659-168">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="d9659-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9659-169">Response</span></span>
<span data-ttu-id="d9659-170">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9659-170">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9659-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9659-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9659-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9659-172">Request</span></span>
<span data-ttu-id="d9659-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9659-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d9659-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9659-174">Response</span></span>
<span data-ttu-id="d9659-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9659-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





