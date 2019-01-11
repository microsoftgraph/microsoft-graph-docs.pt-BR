---
title: Atualizar targetedManagedAppConfiguration
description: Atualizar as propriedades de um objeto targetedManagedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 77f75233ad54e9d26110640946be7cdab014cb8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813465"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="7611f-103">Atualizar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7611f-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="7611f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7611f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7611f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7611f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7611f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7611f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7611f-107">Atualizar as propriedades de um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7611f-107">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7611f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7611f-108">Prerequisites</span></span>
<span data-ttu-id="7611f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7611f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7611f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7611f-111">Permission type</span></span>|<span data-ttu-id="7611f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7611f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7611f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7611f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7611f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7611f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7611f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7611f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7611f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7611f-116">Not supported.</span></span>|
|<span data-ttu-id="7611f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7611f-117">Application</span></span>|<span data-ttu-id="7611f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7611f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7611f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7611f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7611f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7611f-120">Request headers</span></span>
|<span data-ttu-id="7611f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7611f-121">Header</span></span>|<span data-ttu-id="7611f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7611f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7611f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7611f-123">Authorization</span></span>|<span data-ttu-id="7611f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7611f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7611f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7611f-125">Accept</span></span>|<span data-ttu-id="7611f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7611f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7611f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7611f-127">Request body</span></span>
<span data-ttu-id="7611f-128">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7611f-128">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="7611f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7611f-129">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="7611f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7611f-130">Property</span></span>|<span data-ttu-id="7611f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7611f-131">Type</span></span>|<span data-ttu-id="7611f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7611f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7611f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="7611f-133">displayName</span></span>|<span data-ttu-id="7611f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7611f-134">String</span></span>|<span data-ttu-id="7611f-135">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="7611f-135">Policy display name.</span></span> <span data-ttu-id="7611f-136">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7611f-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7611f-137">description</span><span class="sxs-lookup"><span data-stu-id="7611f-137">description</span></span>|<span data-ttu-id="7611f-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7611f-138">String</span></span>|<span data-ttu-id="7611f-139">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="7611f-139">The policy's description.</span></span> <span data-ttu-id="7611f-140">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7611f-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7611f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7611f-141">createdDateTime</span></span>|<span data-ttu-id="7611f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7611f-142">DateTimeOffset</span></span>|<span data-ttu-id="7611f-143">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="7611f-143">The date and time the policy was created.</span></span> <span data-ttu-id="7611f-144">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7611f-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7611f-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7611f-145">lastModifiedDateTime</span></span>|<span data-ttu-id="7611f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7611f-146">DateTimeOffset</span></span>|<span data-ttu-id="7611f-147">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="7611f-147">Last time the policy was modified.</span></span> <span data-ttu-id="7611f-148">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7611f-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7611f-149">id</span><span class="sxs-lookup"><span data-stu-id="7611f-149">id</span></span>|<span data-ttu-id="7611f-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7611f-150">String</span></span>|<span data-ttu-id="7611f-151">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7611f-151">Key of the entity.</span></span> <span data-ttu-id="7611f-152">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7611f-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7611f-153">version</span><span class="sxs-lookup"><span data-stu-id="7611f-153">version</span></span>|<span data-ttu-id="7611f-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7611f-154">String</span></span>|<span data-ttu-id="7611f-155">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="7611f-155">Version of the entity.</span></span> <span data-ttu-id="7611f-156">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7611f-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7611f-157">customSettings</span><span class="sxs-lookup"><span data-stu-id="7611f-157">customSettings</span></span>|<span data-ttu-id="7611f-158">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="7611f-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7611f-159">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7611f-159">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="7611f-160">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="7611f-160">deployedAppCount</span></span>|<span data-ttu-id="7611f-161">Int32</span><span class="sxs-lookup"><span data-stu-id="7611f-161">Int32</span></span>|<span data-ttu-id="7611f-162">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="7611f-162">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="7611f-163">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7611f-163">isAssigned</span></span>|<span data-ttu-id="7611f-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="7611f-164">Boolean</span></span>|<span data-ttu-id="7611f-165">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="7611f-165">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="7611f-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="7611f-166">Response</span></span>
<span data-ttu-id="7611f-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7611f-167">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7611f-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7611f-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="7611f-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7611f-169">Request</span></span>
<span data-ttu-id="7611f-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7611f-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 382

{
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="7611f-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="7611f-171">Response</span></span>
<span data-ttu-id="7611f-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7611f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





