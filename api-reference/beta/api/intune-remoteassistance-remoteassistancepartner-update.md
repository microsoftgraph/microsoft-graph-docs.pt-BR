---
title: Atualizar remoteAssistancePartner
description: Atualizar as propriedades de um objeto remoteAssistancePartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f8efa55477402748578a7198dec5ba6a3008ab2e
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178434"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="c4f8d-103">Atualizar remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="c4f8d-103">Update remoteAssistancePartner</span></span>

<span data-ttu-id="c4f8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4f8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4f8d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4f8d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4f8d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4f8d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4f8d-107">Atualizar as propriedades de um objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="c4f8d-107">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4f8d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4f8d-108">Prerequisites</span></span>
<span data-ttu-id="c4f8d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4f8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4f8d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4f8d-111">Permission type</span></span>|<span data-ttu-id="c4f8d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4f8d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4f8d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4f8d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4f8d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4f8d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c4f8d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4f8d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4f8d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4f8d-116">Not supported.</span></span>|
|<span data-ttu-id="c4f8d-117">Application</span><span class="sxs-lookup"><span data-stu-id="c4f8d-117">Application</span></span>|<span data-ttu-id="c4f8d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4f8d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4f8d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4f8d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="c4f8d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4f8d-120">Request headers</span></span>
|<span data-ttu-id="c4f8d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4f8d-121">Header</span></span>|<span data-ttu-id="c4f8d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c4f8d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4f8d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4f8d-123">Authorization</span></span>|<span data-ttu-id="c4f8d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4f8d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4f8d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4f8d-125">Accept</span></span>|<span data-ttu-id="c4f8d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4f8d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4f8d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4f8d-127">Request body</span></span>
<span data-ttu-id="c4f8d-128">No corpo da solicitação, forneça uma representação JSON do objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="c4f8d-128">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="c4f8d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="c4f8d-129">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="c4f8d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4f8d-130">Property</span></span>|<span data-ttu-id="c4f8d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4f8d-131">Type</span></span>|<span data-ttu-id="c4f8d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4f8d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4f8d-133">id</span><span class="sxs-lookup"><span data-stu-id="c4f8d-133">id</span></span>|<span data-ttu-id="c4f8d-134">String</span><span class="sxs-lookup"><span data-stu-id="c4f8d-134">String</span></span>|<span data-ttu-id="c4f8d-135">O identificador exclusivo do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c4f8d-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="c4f8d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c4f8d-136">displayName</span></span>|<span data-ttu-id="c4f8d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4f8d-137">String</span></span>|<span data-ttu-id="c4f8d-138">Nome de exibição do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c4f8d-138">Display name of the partner.</span></span>|
|<span data-ttu-id="c4f8d-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="c4f8d-139">onboardingUrl</span></span>|<span data-ttu-id="c4f8d-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4f8d-140">String</span></span>|<span data-ttu-id="c4f8d-141">URL do portal de integração do parceiro, no qual um administrador pode configurar o serviço de assistência remota.</span><span class="sxs-lookup"><span data-stu-id="c4f8d-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="c4f8d-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="c4f8d-142">onboardingStatus</span></span>|[<span data-ttu-id="c4f8d-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="c4f8d-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="c4f8d-144">Uma descrição amigável do status atual do conector do TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="c4f8d-144">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="c4f8d-145">Os valores possíveis são: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="c4f8d-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="c4f8d-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="c4f8d-146">lastConnectionDateTime</span></span>|<span data-ttu-id="c4f8d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4f8d-147">DateTimeOffset</span></span>|<span data-ttu-id="c4f8d-148">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="c4f8d-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="c4f8d-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4f8d-149">Response</span></span>
<span data-ttu-id="c4f8d-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4f8d-150">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4f8d-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4f8d-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4f8d-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4f8d-152">Request</span></span>
<span data-ttu-id="c4f8d-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4f8d-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
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

### <a name="response"></a><span data-ttu-id="c4f8d-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4f8d-154">Response</span></span>
<span data-ttu-id="c4f8d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4f8d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



