---
title: Atualizar depOnboardingSetting
description: Atualize as propriedades de um objeto depOnboardingSetting.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 78d3138950776dd74a055fbb00339e9e69b5f0f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412286"
---
# <a name="update-deponboardingsetting"></a><span data-ttu-id="156bc-103">Atualizar depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="156bc-103">Update depOnboardingSetting</span></span>

> <span data-ttu-id="156bc-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="156bc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="156bc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="156bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="156bc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="156bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="156bc-107">Atualize as propriedades de um objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="156bc-107">Update the properties of a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="156bc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="156bc-108">Prerequisites</span></span>
<span data-ttu-id="156bc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="156bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="156bc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="156bc-111">Permission type</span></span>|<span data-ttu-id="156bc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="156bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="156bc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="156bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="156bc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="156bc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="156bc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="156bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="156bc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="156bc-116">Not supported.</span></span>|
|<span data-ttu-id="156bc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="156bc-117">Application</span></span>|<span data-ttu-id="156bc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="156bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="156bc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="156bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a><span data-ttu-id="156bc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="156bc-120">Request headers</span></span>
|<span data-ttu-id="156bc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="156bc-121">Header</span></span>|<span data-ttu-id="156bc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="156bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="156bc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="156bc-123">Authorization</span></span>|<span data-ttu-id="156bc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="156bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="156bc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="156bc-125">Accept</span></span>|<span data-ttu-id="156bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="156bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="156bc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="156bc-127">Request body</span></span>
<span data-ttu-id="156bc-128">No corpo da solicitação, fornece uma representação JSON para o objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="156bc-128">In the request body, supply a JSON representation for the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

<span data-ttu-id="156bc-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span><span class="sxs-lookup"><span data-stu-id="156bc-129">The following table shows the properties that are required when you create the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span></span>

|<span data-ttu-id="156bc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="156bc-130">Property</span></span>|<span data-ttu-id="156bc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="156bc-131">Type</span></span>|<span data-ttu-id="156bc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="156bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="156bc-133">id</span><span class="sxs-lookup"><span data-stu-id="156bc-133">id</span></span>|<span data-ttu-id="156bc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="156bc-134">String</span></span>|<span data-ttu-id="156bc-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="156bc-135">UUID for the object</span></span>|
|<span data-ttu-id="156bc-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="156bc-136">appleIdentifier</span></span>|<span data-ttu-id="156bc-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="156bc-137">String</span></span>|<span data-ttu-id="156bc-138">A ID do Apple usada para obter o token atual.</span><span class="sxs-lookup"><span data-stu-id="156bc-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="156bc-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="156bc-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="156bc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="156bc-140">DateTimeOffset</span></span>|<span data-ttu-id="156bc-141">Quando o token irá expirar.</span><span class="sxs-lookup"><span data-stu-id="156bc-141">When the token will expire.</span></span>|
|<span data-ttu-id="156bc-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="156bc-142">lastModifiedDateTime</span></span>|<span data-ttu-id="156bc-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="156bc-143">DateTimeOffset</span></span>|<span data-ttu-id="156bc-144">Quando o serviço foi onboarded.</span><span class="sxs-lookup"><span data-stu-id="156bc-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="156bc-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="156bc-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="156bc-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="156bc-146">DateTimeOffset</span></span>|<span data-ttu-id="156bc-147">Quando o syned última do serviço com Intune</span><span class="sxs-lookup"><span data-stu-id="156bc-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="156bc-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="156bc-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="156bc-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="156bc-149">DateTimeOffset</span></span>|<span data-ttu-id="156bc-150">Quando o Intune solicitado último uma sincronização.</span><span class="sxs-lookup"><span data-stu-id="156bc-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="156bc-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="156bc-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="156bc-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="156bc-152">Boolean</span></span>|<span data-ttu-id="156bc-153">Ou não o compartilhamento token do Dep está habilitado com o serviço de sincronização de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="156bc-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="156bc-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="156bc-154">lastSyncErrorCode</span></span>|<span data-ttu-id="156bc-155">Int32</span><span class="sxs-lookup"><span data-stu-id="156bc-155">Int32</span></span>|<span data-ttu-id="156bc-156">Código de erro relatado pelo Apple durante a última sincronização dep.</span><span class="sxs-lookup"><span data-stu-id="156bc-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="156bc-157">tokenType</span><span class="sxs-lookup"><span data-stu-id="156bc-157">tokenType</span></span>|[<span data-ttu-id="156bc-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="156bc-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="156bc-159">Obtém ou define o tipo de Token do Dep.</span><span class="sxs-lookup"><span data-stu-id="156bc-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="156bc-160">Os valores possíveis são: `none`, `dep`, `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="156bc-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="156bc-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="156bc-161">tokenName</span></span>|<span data-ttu-id="156bc-162">String</span><span class="sxs-lookup"><span data-stu-id="156bc-162">String</span></span>|<span data-ttu-id="156bc-163">Nome amigável para o Token de Dep</span><span class="sxs-lookup"><span data-stu-id="156bc-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="156bc-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="156bc-164">syncedDeviceCount</span></span>|<span data-ttu-id="156bc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="156bc-165">Int32</span></span>|<span data-ttu-id="156bc-166">Obtém sincronizados contagem de dispositivo</span><span class="sxs-lookup"><span data-stu-id="156bc-166">Gets synced device count</span></span>|
|<span data-ttu-id="156bc-167">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="156bc-167">dataSharingConsentGranted</span></span>|<span data-ttu-id="156bc-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="156bc-168">Boolean</span></span>|<span data-ttu-id="156bc-169">Concedido consentimento para o compartilhamento de dados com Apple Dep Service</span><span class="sxs-lookup"><span data-stu-id="156bc-169">Consent granted for data sharing with Apple Dep Service</span></span>|



## <a name="response"></a><span data-ttu-id="156bc-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="156bc-170">Response</span></span>
<span data-ttu-id="156bc-171">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="156bc-171">If successful, this method returns a `200 OK` response code and an updated [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="156bc-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="156bc-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="156bc-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="156bc-173">Request</span></span>
<span data-ttu-id="156bc-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="156bc-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 514

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true
}
```

### <a name="response"></a><span data-ttu-id="156bc-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="156bc-175">Response</span></span>
<span data-ttu-id="156bc-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="156bc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 627

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "40342229-2229-4034-2922-344029223440",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true
}
```




