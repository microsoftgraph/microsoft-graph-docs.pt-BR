---
title: Criar remoteAssistancePartner
description: Criar um novo objeto remoteAssistancePartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c218d01a2c8c3b60a6de75a677f722d0a49c05e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698383"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="d4cf2-103">Criar remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="d4cf2-103">Create remoteAssistancePartner</span></span>

<span data-ttu-id="d4cf2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4cf2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4cf2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4cf2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4cf2-107">Criar um novo objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="d4cf2-107">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4cf2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4cf2-108">Prerequisites</span></span>
<span data-ttu-id="d4cf2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4cf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4cf2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4cf2-111">Permission type</span></span>|<span data-ttu-id="d4cf2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4cf2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4cf2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4cf2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4cf2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4cf2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d4cf2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4cf2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4cf2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-116">Not supported.</span></span>|
|<span data-ttu-id="d4cf2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4cf2-117">Application</span></span>|<span data-ttu-id="d4cf2-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4cf2-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4cf2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4cf2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="d4cf2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4cf2-120">Request headers</span></span>
|<span data-ttu-id="d4cf2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4cf2-121">Header</span></span>|<span data-ttu-id="d4cf2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d4cf2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4cf2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4cf2-123">Authorization</span></span>|<span data-ttu-id="d4cf2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4cf2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d4cf2-125">Accept</span></span>|<span data-ttu-id="d4cf2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4cf2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4cf2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4cf2-127">Request body</span></span>
<span data-ttu-id="d4cf2-128">No corpo da solicitação, forneça uma representação JSON do objeto remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-128">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="d4cf2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-129">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="d4cf2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4cf2-130">Property</span></span>|<span data-ttu-id="d4cf2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4cf2-131">Type</span></span>|<span data-ttu-id="d4cf2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4cf2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4cf2-133">id</span><span class="sxs-lookup"><span data-stu-id="d4cf2-133">id</span></span>|<span data-ttu-id="d4cf2-134">String</span><span class="sxs-lookup"><span data-stu-id="d4cf2-134">String</span></span>|<span data-ttu-id="d4cf2-135">O identificador exclusivo do parceiro.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="d4cf2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d4cf2-136">displayName</span></span>|<span data-ttu-id="d4cf2-137">String</span><span class="sxs-lookup"><span data-stu-id="d4cf2-137">String</span></span>|<span data-ttu-id="d4cf2-138">Nome de exibição do parceiro.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-138">Display name of the partner.</span></span>|
|<span data-ttu-id="d4cf2-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="d4cf2-139">onboardingUrl</span></span>|<span data-ttu-id="d4cf2-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4cf2-140">String</span></span>|<span data-ttu-id="d4cf2-141">URL do portal de integração do parceiro, no qual um administrador pode configurar o serviço de assistência remota.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="d4cf2-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="d4cf2-142">onboardingStatus</span></span>|[<span data-ttu-id="d4cf2-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="d4cf2-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="d4cf2-144">Uma descrição amigável do status atual do conector do TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-144">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="d4cf2-145">Os valores possíveis são: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="d4cf2-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="d4cf2-146">lastConnectionDateTime</span></span>|<span data-ttu-id="d4cf2-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4cf2-147">DateTimeOffset</span></span>|<span data-ttu-id="d4cf2-148">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|
|<span data-ttu-id="d4cf2-149">onboardingRequestExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="d4cf2-149">onboardingRequestExpiryDateTime</span></span>|<span data-ttu-id="d4cf2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4cf2-150">DateTimeOffset</span></span>|<span data-ttu-id="d4cf2-151">Quando o OnboardingStatus está em integração, esta é a data e hora em que a solicitação de integração expira.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-151">When the OnboardingStatus is Onboarding, This is the date time when the onboarding request expires.</span></span>|



## <a name="response"></a><span data-ttu-id="d4cf2-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4cf2-152">Response</span></span>
<span data-ttu-id="d4cf2-153">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-153">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4cf2-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4cf2-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4cf2-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4cf2-155">Request</span></span>
<span data-ttu-id="d4cf2-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners
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

### <a name="response"></a><span data-ttu-id="d4cf2-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4cf2-157">Response</span></span>
<span data-ttu-id="d4cf2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4cf2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





