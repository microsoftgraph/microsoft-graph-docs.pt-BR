---
title: Atualizar targetedManagedAppConfiguration
description: Atualizar as propriedades de um objeto targetedManagedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3e9cf1f31539789109bc7c538c2a318ae8d685e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916100"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="6a4e4-103">Atualizar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6a4e4-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="6a4e4-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6a4e4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a4e4-105">Atualizar as propriedades de um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a4e4-105">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6a4e4-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a4e4-106">Prerequisites</span></span>
<span data-ttu-id="6a4e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a4e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a4e4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a4e4-109">Permission type</span></span>|<span data-ttu-id="6a4e4-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a4e4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a4e4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a4e4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6a4e4-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a4e4-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6a4e4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a4e4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a4e4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a4e4-114">Not supported.</span></span>|
|<span data-ttu-id="6a4e4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a4e4-115">Application</span></span>|<span data-ttu-id="6a4e4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a4e4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a4e4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a4e4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6a4e4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a4e4-118">Request headers</span></span>
|<span data-ttu-id="6a4e4-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a4e4-119">Header</span></span>|<span data-ttu-id="6a4e4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6a4e4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a4e4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a4e4-121">Authorization</span></span>|<span data-ttu-id="6a4e4-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a4e4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a4e4-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a4e4-123">Accept</span></span>|<span data-ttu-id="6a4e4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6a4e4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a4e4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a4e4-125">Request body</span></span>
<span data-ttu-id="6a4e4-126">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a4e4-126">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="6a4e4-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a4e4-127">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="6a4e4-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a4e4-128">Property</span></span>|<span data-ttu-id="6a4e4-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a4e4-129">Type</span></span>|<span data-ttu-id="6a4e4-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a4e4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a4e4-131">displayName</span><span class="sxs-lookup"><span data-stu-id="6a4e4-131">displayName</span></span>|<span data-ttu-id="6a4e4-132">String</span><span class="sxs-lookup"><span data-stu-id="6a4e4-132">String</span></span>|<span data-ttu-id="6a4e4-133">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="6a4e4-133">Policy display name.</span></span> <span data-ttu-id="6a4e4-134">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6a4e4-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6a4e4-135">description</span><span class="sxs-lookup"><span data-stu-id="6a4e4-135">description</span></span>|<span data-ttu-id="6a4e4-136">String</span><span class="sxs-lookup"><span data-stu-id="6a4e4-136">String</span></span>|<span data-ttu-id="6a4e4-137">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="6a4e4-137">The policy's description.</span></span> <span data-ttu-id="6a4e4-138">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6a4e4-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6a4e4-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a4e4-139">createdDateTime</span></span>|<span data-ttu-id="6a4e4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a4e4-140">DateTimeOffset</span></span>|<span data-ttu-id="6a4e4-141">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="6a4e4-141">The date and time the policy was created.</span></span> <span data-ttu-id="6a4e4-142">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6a4e4-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6a4e4-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a4e4-143">lastModifiedDateTime</span></span>|<span data-ttu-id="6a4e4-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a4e4-144">DateTimeOffset</span></span>|<span data-ttu-id="6a4e4-145">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="6a4e4-145">Last time the policy was modified.</span></span> <span data-ttu-id="6a4e4-146">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6a4e4-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6a4e4-147">id</span><span class="sxs-lookup"><span data-stu-id="6a4e4-147">id</span></span>|<span data-ttu-id="6a4e4-148">String</span><span class="sxs-lookup"><span data-stu-id="6a4e4-148">String</span></span>|<span data-ttu-id="6a4e4-149">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6a4e4-149">Key of the entity.</span></span> <span data-ttu-id="6a4e4-150">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6a4e4-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6a4e4-151">version</span><span class="sxs-lookup"><span data-stu-id="6a4e4-151">version</span></span>|<span data-ttu-id="6a4e4-152">String</span><span class="sxs-lookup"><span data-stu-id="6a4e4-152">String</span></span>|<span data-ttu-id="6a4e4-153">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="6a4e4-153">Version of the entity.</span></span> <span data-ttu-id="6a4e4-154">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6a4e4-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6a4e4-155">customSettings</span><span class="sxs-lookup"><span data-stu-id="6a4e4-155">customSettings</span></span>|<span data-ttu-id="6a4e4-156">Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6a4e4-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6a4e4-157">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a4e4-157">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="6a4e4-158">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="6a4e4-158">deployedAppCount</span></span>|<span data-ttu-id="6a4e4-159">Int32</span><span class="sxs-lookup"><span data-stu-id="6a4e4-159">Int32</span></span>|<span data-ttu-id="6a4e4-160">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="6a4e4-160">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="6a4e4-161">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6a4e4-161">isAssigned</span></span>|<span data-ttu-id="6a4e4-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a4e4-162">Boolean</span></span>|<span data-ttu-id="6a4e4-163">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="6a4e4-163">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="6a4e4-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a4e4-164">Response</span></span>
<span data-ttu-id="6a4e4-165">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a4e4-165">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a4e4-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a4e4-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="6a4e4-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a4e4-167">Request</span></span>
<span data-ttu-id="6a4e4-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a4e4-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6a4e4-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a4e4-169">Response</span></span>
<span data-ttu-id="6a4e4-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a4e4-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



