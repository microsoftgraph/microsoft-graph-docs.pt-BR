---
title: Atualizar remoteAssistancePartner
description: Atualizar as propriedades de um objeto remoteAssistancePartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f969d3fa1c5adbc5e6be5da504cce302963f5260
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989634"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="4475b-103">Atualizar remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="4475b-103">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="4475b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4475b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4475b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4475b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4475b-106">Atualizar as propriedades de um objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="4475b-106">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4475b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4475b-107">Prerequisites</span></span>
<span data-ttu-id="4475b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4475b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4475b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4475b-110">Permission type</span></span>|<span data-ttu-id="4475b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4475b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4475b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4475b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4475b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4475b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4475b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4475b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4475b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4475b-115">Not supported.</span></span>|
|<span data-ttu-id="4475b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4475b-116">Application</span></span>|<span data-ttu-id="4475b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4475b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4475b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4475b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="4475b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4475b-119">Request headers</span></span>
|<span data-ttu-id="4475b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4475b-120">Header</span></span>|<span data-ttu-id="4475b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4475b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4475b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4475b-122">Authorization</span></span>|<span data-ttu-id="4475b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4475b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4475b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4475b-124">Accept</span></span>|<span data-ttu-id="4475b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4475b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4475b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4475b-126">Request body</span></span>
<span data-ttu-id="4475b-127">No corpo da solicitação, forneça uma representação JSON do objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="4475b-127">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="4475b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="4475b-128">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="4475b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4475b-129">Property</span></span>|<span data-ttu-id="4475b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4475b-130">Type</span></span>|<span data-ttu-id="4475b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4475b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4475b-132">id</span><span class="sxs-lookup"><span data-stu-id="4475b-132">id</span></span>|<span data-ttu-id="4475b-133">String</span><span class="sxs-lookup"><span data-stu-id="4475b-133">String</span></span>|<span data-ttu-id="4475b-134">O identificador exclusivo do parceiro.</span><span class="sxs-lookup"><span data-stu-id="4475b-134">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="4475b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4475b-135">displayName</span></span>|<span data-ttu-id="4475b-136">String</span><span class="sxs-lookup"><span data-stu-id="4475b-136">String</span></span>|<span data-ttu-id="4475b-137">Nome de exibição do parceiro.</span><span class="sxs-lookup"><span data-stu-id="4475b-137">Display name of the partner.</span></span>|
|<span data-ttu-id="4475b-138">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="4475b-138">onboardingUrl</span></span>|<span data-ttu-id="4475b-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4475b-139">String</span></span>|<span data-ttu-id="4475b-140">URL do portal de integração do parceiro, no qual um administrador pode configurar o serviço de assistência remota.</span><span class="sxs-lookup"><span data-stu-id="4475b-140">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="4475b-141">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="4475b-141">onboardingStatus</span></span>|[<span data-ttu-id="4475b-142">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="4475b-142">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="4475b-143">Uma descrição amigável do status atual do conector do TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="4475b-143">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="4475b-144">Os valores possíveis são: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="4475b-144">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="4475b-145">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="4475b-145">lastConnectionDateTime</span></span>|<span data-ttu-id="4475b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4475b-146">DateTimeOffset</span></span>|<span data-ttu-id="4475b-147">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="4475b-147">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="4475b-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="4475b-148">Response</span></span>
<span data-ttu-id="4475b-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4475b-149">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4475b-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4475b-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="4475b-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4475b-151">Request</span></span>
<span data-ttu-id="4475b-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4475b-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4475b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="4475b-153">Response</span></span>
<span data-ttu-id="4475b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4475b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





