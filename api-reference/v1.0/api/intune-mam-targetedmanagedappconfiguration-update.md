---
title: Atualizar targetedManagedAppConfiguration
description: Atualizar as propriedades de um objeto targetedManagedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8d420324572da4e9459839184325bd4f70512f47
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43397982"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="1880b-103">Atualizar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1880b-103">Update targetedManagedAppConfiguration</span></span>

<span data-ttu-id="1880b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1880b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1880b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1880b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1880b-106">Atualizar as propriedades de um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1880b-106">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1880b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1880b-107">Prerequisites</span></span>
<span data-ttu-id="1880b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1880b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1880b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1880b-110">Permission type</span></span>|<span data-ttu-id="1880b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1880b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1880b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1880b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1880b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1880b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1880b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1880b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1880b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1880b-115">Not supported.</span></span>|
|<span data-ttu-id="1880b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1880b-116">Application</span></span>|<span data-ttu-id="1880b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1880b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1880b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1880b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1880b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1880b-119">Request headers</span></span>
|<span data-ttu-id="1880b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1880b-120">Header</span></span>|<span data-ttu-id="1880b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1880b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1880b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1880b-122">Authorization</span></span>|<span data-ttu-id="1880b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1880b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1880b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1880b-124">Accept</span></span>|<span data-ttu-id="1880b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1880b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1880b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1880b-126">Request body</span></span>
<span data-ttu-id="1880b-127">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1880b-127">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="1880b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1880b-128">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="1880b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1880b-129">Property</span></span>|<span data-ttu-id="1880b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1880b-130">Type</span></span>|<span data-ttu-id="1880b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1880b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1880b-132">displayName</span><span class="sxs-lookup"><span data-stu-id="1880b-132">displayName</span></span>|<span data-ttu-id="1880b-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1880b-133">String</span></span>|<span data-ttu-id="1880b-134">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="1880b-134">Policy display name.</span></span> <span data-ttu-id="1880b-135">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1880b-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1880b-136">description</span><span class="sxs-lookup"><span data-stu-id="1880b-136">description</span></span>|<span data-ttu-id="1880b-137">String</span><span class="sxs-lookup"><span data-stu-id="1880b-137">String</span></span>|<span data-ttu-id="1880b-138">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="1880b-138">The policy's description.</span></span> <span data-ttu-id="1880b-139">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1880b-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1880b-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1880b-140">createdDateTime</span></span>|<span data-ttu-id="1880b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1880b-141">DateTimeOffset</span></span>|<span data-ttu-id="1880b-142">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="1880b-142">The date and time the policy was created.</span></span> <span data-ttu-id="1880b-143">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1880b-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1880b-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1880b-144">lastModifiedDateTime</span></span>|<span data-ttu-id="1880b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1880b-145">DateTimeOffset</span></span>|<span data-ttu-id="1880b-146">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="1880b-146">Last time the policy was modified.</span></span> <span data-ttu-id="1880b-147">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1880b-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1880b-148">id</span><span class="sxs-lookup"><span data-stu-id="1880b-148">id</span></span>|<span data-ttu-id="1880b-149">String</span><span class="sxs-lookup"><span data-stu-id="1880b-149">String</span></span>|<span data-ttu-id="1880b-150">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1880b-150">Key of the entity.</span></span> <span data-ttu-id="1880b-151">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1880b-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1880b-152">version</span><span class="sxs-lookup"><span data-stu-id="1880b-152">version</span></span>|<span data-ttu-id="1880b-153">String</span><span class="sxs-lookup"><span data-stu-id="1880b-153">String</span></span>|<span data-ttu-id="1880b-154">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="1880b-154">Version of the entity.</span></span> <span data-ttu-id="1880b-155">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1880b-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1880b-156">customSettings</span><span class="sxs-lookup"><span data-stu-id="1880b-156">customSettings</span></span>|<span data-ttu-id="1880b-157">Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="1880b-157">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="1880b-158">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1880b-158">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="1880b-159">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="1880b-159">deployedAppCount</span></span>|<span data-ttu-id="1880b-160">Int32</span><span class="sxs-lookup"><span data-stu-id="1880b-160">Int32</span></span>|<span data-ttu-id="1880b-161">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="1880b-161">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="1880b-162">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1880b-162">isAssigned</span></span>|<span data-ttu-id="1880b-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="1880b-163">Boolean</span></span>|<span data-ttu-id="1880b-164">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="1880b-164">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="1880b-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="1880b-165">Response</span></span>
<span data-ttu-id="1880b-166">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1880b-166">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1880b-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1880b-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="1880b-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1880b-168">Request</span></span>
<span data-ttu-id="1880b-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1880b-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1880b-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="1880b-170">Response</span></span>
<span data-ttu-id="1880b-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1880b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






