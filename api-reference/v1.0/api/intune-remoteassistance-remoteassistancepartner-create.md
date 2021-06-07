---
title: Criar remoteAssistancePartner
description: Criar um novo objeto remoteAssistancePartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1a1da12ef0e782adfb1b80a15cb5a3bfad203ebf
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759027"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="fb458-103">Criar remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="fb458-103">Create remoteAssistancePartner</span></span>

<span data-ttu-id="fb458-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb458-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb458-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb458-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb458-106">Criar um novo objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="fb458-106">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb458-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb458-107">Prerequisites</span></span>
<span data-ttu-id="fb458-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb458-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb458-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb458-110">Permission type</span></span>|<span data-ttu-id="fb458-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb458-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb458-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb458-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fb458-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb458-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fb458-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb458-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb458-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb458-115">Not supported.</span></span>|
|<span data-ttu-id="fb458-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb458-116">Application</span></span>|<span data-ttu-id="fb458-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb458-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb458-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb458-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="fb458-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb458-119">Request headers</span></span>
|<span data-ttu-id="fb458-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb458-120">Header</span></span>|<span data-ttu-id="fb458-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fb458-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb458-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb458-122">Authorization</span></span>|<span data-ttu-id="fb458-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb458-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb458-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb458-124">Accept</span></span>|<span data-ttu-id="fb458-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb458-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb458-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb458-126">Request body</span></span>
<span data-ttu-id="fb458-127">No corpo da solicitação, forneça uma representação JSON do objeto remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="fb458-127">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="fb458-128">A tabela a seguir mostra as propriedades que são necessárias ao criar remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="fb458-128">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="fb458-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb458-129">Property</span></span>|<span data-ttu-id="fb458-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb458-130">Type</span></span>|<span data-ttu-id="fb458-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb458-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb458-132">id</span><span class="sxs-lookup"><span data-stu-id="fb458-132">id</span></span>|<span data-ttu-id="fb458-133">String</span><span class="sxs-lookup"><span data-stu-id="fb458-133">String</span></span>|<span data-ttu-id="fb458-134">O identificador exclusivo do parceiro.</span><span class="sxs-lookup"><span data-stu-id="fb458-134">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="fb458-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fb458-135">displayName</span></span>|<span data-ttu-id="fb458-136">String</span><span class="sxs-lookup"><span data-stu-id="fb458-136">String</span></span>|<span data-ttu-id="fb458-137">Nome de exibição do parceiro.</span><span class="sxs-lookup"><span data-stu-id="fb458-137">Display name of the partner.</span></span>|
|<span data-ttu-id="fb458-138">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="fb458-138">onboardingUrl</span></span>|<span data-ttu-id="fb458-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb458-139">String</span></span>|<span data-ttu-id="fb458-140">URL do portal de integração do parceiro, no qual um administrador pode configurar o serviço de assistência remota.</span><span class="sxs-lookup"><span data-stu-id="fb458-140">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="fb458-141">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="fb458-141">onboardingStatus</span></span>|[<span data-ttu-id="fb458-142">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="fb458-142">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="fb458-143">Uma descrição amigável do status atual do conector teamViewer.</span><span class="sxs-lookup"><span data-stu-id="fb458-143">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="fb458-144">Os valores possíveis são: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="fb458-144">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="fb458-145">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="fb458-145">lastConnectionDateTime</span></span>|<span data-ttu-id="fb458-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb458-146">DateTimeOffset</span></span>|<span data-ttu-id="fb458-147">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="fb458-147">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="fb458-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb458-148">Response</span></span>
<span data-ttu-id="fb458-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb458-149">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb458-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb458-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb458-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb458-151">Request</span></span>
<span data-ttu-id="fb458-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb458-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="fb458-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb458-153">Response</span></span>
<span data-ttu-id="fb458-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb458-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```




