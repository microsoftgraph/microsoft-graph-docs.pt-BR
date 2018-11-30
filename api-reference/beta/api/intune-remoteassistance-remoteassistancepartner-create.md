---
title: Criar remoteAssistancePartner
description: Criar um novo objeto remoteAssistancePartner.
ms.openlocfilehash: 1d6630622a3115cc7429547677c38e95bf96893a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035721"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="a710c-103">Criar remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="a710c-103">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="a710c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a710c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a710c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a710c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a710c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a710c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a710c-107">Criar um novo objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="a710c-107">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a710c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a710c-108">Prerequisites</span></span>
<span data-ttu-id="a710c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a710c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a710c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a710c-111">Permission type</span></span>|<span data-ttu-id="a710c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a710c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a710c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a710c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a710c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a710c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a710c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a710c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a710c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a710c-116">Not supported.</span></span>|
|<span data-ttu-id="a710c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a710c-117">Application</span></span>|<span data-ttu-id="a710c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a710c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a710c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a710c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="a710c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a710c-120">Request headers</span></span>
|<span data-ttu-id="a710c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a710c-121">Header</span></span>|<span data-ttu-id="a710c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a710c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a710c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a710c-123">Authorization</span></span>|<span data-ttu-id="a710c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a710c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a710c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a710c-125">Accept</span></span>|<span data-ttu-id="a710c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a710c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a710c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a710c-127">Request body</span></span>
<span data-ttu-id="a710c-128">No corpo da solicitação, forneça uma representação JSON do objeto remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="a710c-128">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="a710c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="a710c-129">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="a710c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a710c-130">Property</span></span>|<span data-ttu-id="a710c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a710c-131">Type</span></span>|<span data-ttu-id="a710c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a710c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a710c-133">id</span><span class="sxs-lookup"><span data-stu-id="a710c-133">id</span></span>|<span data-ttu-id="a710c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a710c-134">String</span></span>|<span data-ttu-id="a710c-135">O identificador exclusivo do parceiro.</span><span class="sxs-lookup"><span data-stu-id="a710c-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="a710c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a710c-136">displayName</span></span>|<span data-ttu-id="a710c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a710c-137">String</span></span>|<span data-ttu-id="a710c-138">Nome de exibição do parceiro.</span><span class="sxs-lookup"><span data-stu-id="a710c-138">Display name of the partner.</span></span>|
|<span data-ttu-id="a710c-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="a710c-139">onboardingUrl</span></span>|<span data-ttu-id="a710c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a710c-140">String</span></span>|<span data-ttu-id="a710c-141">URL do portal de integração do parceiro, no qual um administrador pode configurar o serviço de assistência remota.</span><span class="sxs-lookup"><span data-stu-id="a710c-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="a710c-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="a710c-142">onboardingStatus</span></span>|[<span data-ttu-id="a710c-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="a710c-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="a710c-144">TBD.</span><span class="sxs-lookup"><span data-stu-id="a710c-144">TBD.</span></span> <span data-ttu-id="a710c-145">Os valores possíveis são: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="a710c-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="a710c-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="a710c-146">lastConnectionDateTime</span></span>|<span data-ttu-id="a710c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a710c-147">DateTimeOffset</span></span>|<span data-ttu-id="a710c-148">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="a710c-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="a710c-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="a710c-149">Response</span></span>
<span data-ttu-id="a710c-150">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a710c-150">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a710c-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a710c-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="a710c-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a710c-152">Request</span></span>
<span data-ttu-id="a710c-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a710c-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners
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

### <a name="response"></a><span data-ttu-id="a710c-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="a710c-154">Response</span></span>
<span data-ttu-id="a710c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a710c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





