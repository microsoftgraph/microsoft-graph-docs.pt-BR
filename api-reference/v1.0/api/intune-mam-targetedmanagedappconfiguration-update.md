---
title: Atualizar targetedManagedAppConfiguration
description: Atualizar as propriedades de um objeto targetedManagedAppConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 39b7c6900fd7249d33eb6708ca07bca41e41c58f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512941"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="2e7f5-103">Atualizar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2e7f5-103">Update targetedManagedAppConfiguration</span></span>

<span data-ttu-id="2e7f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e7f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e7f5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2e7f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e7f5-106">Atualizar as propriedades de um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e7f5-106">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e7f5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2e7f5-107">Prerequisites</span></span>
<span data-ttu-id="2e7f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e7f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e7f5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e7f5-110">Permission type</span></span>|<span data-ttu-id="2e7f5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2e7f5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e7f5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e7f5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2e7f5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e7f5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2e7f5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e7f5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e7f5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e7f5-115">Not supported.</span></span>|
|<span data-ttu-id="2e7f5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e7f5-116">Application</span></span>|<span data-ttu-id="2e7f5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e7f5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e7f5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e7f5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2e7f5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e7f5-119">Request headers</span></span>
|<span data-ttu-id="2e7f5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2e7f5-120">Header</span></span>|<span data-ttu-id="2e7f5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2e7f5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e7f5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e7f5-122">Authorization</span></span>|<span data-ttu-id="2e7f5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e7f5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e7f5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2e7f5-124">Accept</span></span>|<span data-ttu-id="2e7f5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2e7f5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e7f5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e7f5-126">Request body</span></span>
<span data-ttu-id="2e7f5-127">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e7f5-127">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="2e7f5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e7f5-128">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="2e7f5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e7f5-129">Property</span></span>|<span data-ttu-id="2e7f5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e7f5-130">Type</span></span>|<span data-ttu-id="2e7f5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e7f5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e7f5-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2e7f5-132">displayName</span></span>|<span data-ttu-id="2e7f5-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e7f5-133">String</span></span>|<span data-ttu-id="2e7f5-134">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="2e7f5-134">Policy display name.</span></span> <span data-ttu-id="2e7f5-135">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2e7f5-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2e7f5-136">description</span><span class="sxs-lookup"><span data-stu-id="2e7f5-136">description</span></span>|<span data-ttu-id="2e7f5-137">String</span><span class="sxs-lookup"><span data-stu-id="2e7f5-137">String</span></span>|<span data-ttu-id="2e7f5-138">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="2e7f5-138">The policy's description.</span></span> <span data-ttu-id="2e7f5-139">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2e7f5-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2e7f5-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2e7f5-140">createdDateTime</span></span>|<span data-ttu-id="2e7f5-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e7f5-141">DateTimeOffset</span></span>|<span data-ttu-id="2e7f5-142">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="2e7f5-142">The date and time the policy was created.</span></span> <span data-ttu-id="2e7f5-143">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2e7f5-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2e7f5-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e7f5-144">lastModifiedDateTime</span></span>|<span data-ttu-id="2e7f5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e7f5-145">DateTimeOffset</span></span>|<span data-ttu-id="2e7f5-146">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="2e7f5-146">Last time the policy was modified.</span></span> <span data-ttu-id="2e7f5-147">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2e7f5-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2e7f5-148">id</span><span class="sxs-lookup"><span data-stu-id="2e7f5-148">id</span></span>|<span data-ttu-id="2e7f5-149">String</span><span class="sxs-lookup"><span data-stu-id="2e7f5-149">String</span></span>|<span data-ttu-id="2e7f5-150">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2e7f5-150">Key of the entity.</span></span> <span data-ttu-id="2e7f5-151">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2e7f5-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2e7f5-152">version</span><span class="sxs-lookup"><span data-stu-id="2e7f5-152">version</span></span>|<span data-ttu-id="2e7f5-153">String</span><span class="sxs-lookup"><span data-stu-id="2e7f5-153">String</span></span>|<span data-ttu-id="2e7f5-154">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="2e7f5-154">Version of the entity.</span></span> <span data-ttu-id="2e7f5-155">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2e7f5-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2e7f5-156">customSettings</span><span class="sxs-lookup"><span data-stu-id="2e7f5-156">customSettings</span></span>|<span data-ttu-id="2e7f5-157">Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2e7f5-157">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="2e7f5-158">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2e7f5-158">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="2e7f5-159">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="2e7f5-159">deployedAppCount</span></span>|<span data-ttu-id="2e7f5-160">Int32</span><span class="sxs-lookup"><span data-stu-id="2e7f5-160">Int32</span></span>|<span data-ttu-id="2e7f5-161">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="2e7f5-161">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="2e7f5-162">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2e7f5-162">isAssigned</span></span>|<span data-ttu-id="2e7f5-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7f5-163">Boolean</span></span>|<span data-ttu-id="2e7f5-164">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="2e7f5-164">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="2e7f5-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e7f5-165">Response</span></span>
<span data-ttu-id="2e7f5-166">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e7f5-166">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e7f5-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e7f5-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e7f5-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e7f5-168">Request</span></span>
<span data-ttu-id="2e7f5-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e7f5-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
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

### <a name="response"></a><span data-ttu-id="2e7f5-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e7f5-170">Response</span></span>
<span data-ttu-id="2e7f5-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e7f5-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




