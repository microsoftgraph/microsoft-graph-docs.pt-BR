---
title: Criar remoteAssistancePartner
description: Criar um novo objeto remoteAssistancePartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3723a8b7043f37928d4fd72bd272e6934f2af408
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361662"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="e28cd-103">Criar remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="e28cd-103">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="e28cd-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e28cd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e28cd-105">Criar um novo objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="e28cd-105">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e28cd-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e28cd-106">Prerequisites</span></span>
<span data-ttu-id="e28cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e28cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e28cd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e28cd-109">Permission type</span></span>|<span data-ttu-id="e28cd-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e28cd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e28cd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e28cd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e28cd-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e28cd-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e28cd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e28cd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e28cd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e28cd-114">Not supported.</span></span>|
|<span data-ttu-id="e28cd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e28cd-115">Application</span></span>|<span data-ttu-id="e28cd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e28cd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e28cd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e28cd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="e28cd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e28cd-118">Request headers</span></span>
|<span data-ttu-id="e28cd-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e28cd-119">Header</span></span>|<span data-ttu-id="e28cd-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e28cd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e28cd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e28cd-121">Authorization</span></span>|<span data-ttu-id="e28cd-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e28cd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e28cd-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e28cd-123">Accept</span></span>|<span data-ttu-id="e28cd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e28cd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e28cd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e28cd-125">Request body</span></span>
<span data-ttu-id="e28cd-126">No corpo da solicitação, forneça uma representação JSON do objeto remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="e28cd-126">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="e28cd-127">A tabela a seguir mostra as propriedades que são necessárias ao criar remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="e28cd-127">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="e28cd-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e28cd-128">Property</span></span>|<span data-ttu-id="e28cd-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e28cd-129">Type</span></span>|<span data-ttu-id="e28cd-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e28cd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e28cd-131">id</span><span class="sxs-lookup"><span data-stu-id="e28cd-131">id</span></span>|<span data-ttu-id="e28cd-132">String</span><span class="sxs-lookup"><span data-stu-id="e28cd-132">String</span></span>|<span data-ttu-id="e28cd-133">O identificador exclusivo do parceiro.</span><span class="sxs-lookup"><span data-stu-id="e28cd-133">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="e28cd-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e28cd-134">displayName</span></span>|<span data-ttu-id="e28cd-135">String</span><span class="sxs-lookup"><span data-stu-id="e28cd-135">String</span></span>|<span data-ttu-id="e28cd-136">Nome de exibição do parceiro.</span><span class="sxs-lookup"><span data-stu-id="e28cd-136">Display name of the partner.</span></span>|
|<span data-ttu-id="e28cd-137">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="e28cd-137">onboardingUrl</span></span>|<span data-ttu-id="e28cd-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e28cd-138">String</span></span>|<span data-ttu-id="e28cd-139">URL do portal de integração do parceiro, no qual um administrador pode configurar o serviço de assistência remota.</span><span class="sxs-lookup"><span data-stu-id="e28cd-139">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="e28cd-140">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="e28cd-140">onboardingStatus</span></span>|[<span data-ttu-id="e28cd-141">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="e28cd-141">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="e28cd-142">TBD.</span><span class="sxs-lookup"><span data-stu-id="e28cd-142">TBD.</span></span> <span data-ttu-id="e28cd-143">Os valores possíveis são: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="e28cd-143">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="e28cd-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="e28cd-144">lastConnectionDateTime</span></span>|<span data-ttu-id="e28cd-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e28cd-145">DateTimeOffset</span></span>|<span data-ttu-id="e28cd-146">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="e28cd-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="e28cd-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e28cd-147">Response</span></span>
<span data-ttu-id="e28cd-148">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e28cd-148">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e28cd-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e28cd-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="e28cd-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e28cd-150">Request</span></span>
<span data-ttu-id="e28cd-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e28cd-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e28cd-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="e28cd-152">Response</span></span>
<span data-ttu-id="e28cd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e28cd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




