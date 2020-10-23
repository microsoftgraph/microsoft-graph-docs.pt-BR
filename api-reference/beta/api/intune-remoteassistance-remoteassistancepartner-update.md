---
title: Atualizar remoteAssistancePartner
description: Atualizar as propriedades de um objeto remoteAssistancePartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5d1c7ae72b0e59dbe04a4fe5b4e100e4ded03e53
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698334"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="199ee-103">Atualizar remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="199ee-103">Update remoteAssistancePartner</span></span>

<span data-ttu-id="199ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="199ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="199ee-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="199ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="199ee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="199ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="199ee-107">Atualizar as propriedades de um objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="199ee-107">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="199ee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="199ee-108">Prerequisites</span></span>
<span data-ttu-id="199ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="199ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="199ee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="199ee-111">Permission type</span></span>|<span data-ttu-id="199ee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="199ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="199ee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="199ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="199ee-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="199ee-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="199ee-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="199ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="199ee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="199ee-116">Not supported.</span></span>|
|<span data-ttu-id="199ee-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="199ee-117">Application</span></span>|<span data-ttu-id="199ee-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="199ee-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="199ee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="199ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="199ee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="199ee-120">Request headers</span></span>
|<span data-ttu-id="199ee-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="199ee-121">Header</span></span>|<span data-ttu-id="199ee-122">Valor</span><span class="sxs-lookup"><span data-stu-id="199ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="199ee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="199ee-123">Authorization</span></span>|<span data-ttu-id="199ee-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="199ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="199ee-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="199ee-125">Accept</span></span>|<span data-ttu-id="199ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="199ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="199ee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="199ee-127">Request body</span></span>
<span data-ttu-id="199ee-128">No corpo da solicitação, forneça uma representação JSON do objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="199ee-128">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="199ee-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="199ee-129">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="199ee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="199ee-130">Property</span></span>|<span data-ttu-id="199ee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="199ee-131">Type</span></span>|<span data-ttu-id="199ee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="199ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="199ee-133">id</span><span class="sxs-lookup"><span data-stu-id="199ee-133">id</span></span>|<span data-ttu-id="199ee-134">String</span><span class="sxs-lookup"><span data-stu-id="199ee-134">String</span></span>|<span data-ttu-id="199ee-135">O identificador exclusivo do parceiro.</span><span class="sxs-lookup"><span data-stu-id="199ee-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="199ee-136">displayName</span><span class="sxs-lookup"><span data-stu-id="199ee-136">displayName</span></span>|<span data-ttu-id="199ee-137">String</span><span class="sxs-lookup"><span data-stu-id="199ee-137">String</span></span>|<span data-ttu-id="199ee-138">Nome de exibição do parceiro.</span><span class="sxs-lookup"><span data-stu-id="199ee-138">Display name of the partner.</span></span>|
|<span data-ttu-id="199ee-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="199ee-139">onboardingUrl</span></span>|<span data-ttu-id="199ee-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="199ee-140">String</span></span>|<span data-ttu-id="199ee-141">URL do portal de integração do parceiro, no qual um administrador pode configurar o serviço de assistência remota.</span><span class="sxs-lookup"><span data-stu-id="199ee-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="199ee-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="199ee-142">onboardingStatus</span></span>|[<span data-ttu-id="199ee-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="199ee-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="199ee-144">Uma descrição amigável do status atual do conector do TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="199ee-144">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="199ee-145">Os valores possíveis são: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="199ee-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="199ee-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="199ee-146">lastConnectionDateTime</span></span>|<span data-ttu-id="199ee-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="199ee-147">DateTimeOffset</span></span>|<span data-ttu-id="199ee-148">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="199ee-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|
|<span data-ttu-id="199ee-149">onboardingRequestExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="199ee-149">onboardingRequestExpiryDateTime</span></span>|<span data-ttu-id="199ee-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="199ee-150">DateTimeOffset</span></span>|<span data-ttu-id="199ee-151">Quando o OnboardingStatus está em integração, esta é a data e hora em que a solicitação de integração expira.</span><span class="sxs-lookup"><span data-stu-id="199ee-151">When the OnboardingStatus is Onboarding, This is the date time when the onboarding request expires.</span></span>|



## <a name="response"></a><span data-ttu-id="199ee-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="199ee-152">Response</span></span>
<span data-ttu-id="199ee-153">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="199ee-153">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="199ee-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="199ee-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="199ee-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="199ee-155">Request</span></span>
<span data-ttu-id="199ee-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="199ee-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
Content-type: application/json
Content-length: 341

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "onboardingRequestExpiryDateTime": "2017-01-01T00:02:07.7573274-08:00"
}
```

### <a name="response"></a><span data-ttu-id="199ee-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="199ee-157">Response</span></span>
<span data-ttu-id="199ee-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="199ee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 390

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "onboardingRequestExpiryDateTime": "2017-01-01T00:02:07.7573274-08:00"
}
```





