---
title: Atualizar remoteAssistancePartner
description: Atualizar as propriedades de um objeto remoteAssistancePartner.
ms.openlocfilehash: 62647e197d7c4666ce177fff6c2f1fb7dd1271af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035633"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="7ac4a-103">Atualizar remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="7ac4a-103">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="7ac4a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7ac4a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ac4a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7ac4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ac4a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7ac4a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ac4a-107">Atualizar as propriedades de um objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="7ac4a-107">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7ac4a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7ac4a-108">Prerequisites</span></span>
<span data-ttu-id="7ac4a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ac4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ac4a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ac4a-111">Permission type</span></span>|<span data-ttu-id="7ac4a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7ac4a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ac4a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ac4a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ac4a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ac4a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7ac4a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ac4a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ac4a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ac4a-116">Not supported.</span></span>|
|<span data-ttu-id="7ac4a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ac4a-117">Application</span></span>|<span data-ttu-id="7ac4a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ac4a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ac4a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ac4a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="7ac4a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ac4a-120">Request headers</span></span>
|<span data-ttu-id="7ac4a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ac4a-121">Header</span></span>|<span data-ttu-id="7ac4a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7ac4a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ac4a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ac4a-123">Authorization</span></span>|<span data-ttu-id="7ac4a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ac4a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ac4a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7ac4a-125">Accept</span></span>|<span data-ttu-id="7ac4a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ac4a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ac4a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ac4a-127">Request body</span></span>
<span data-ttu-id="7ac4a-128">No corpo da solicitação, forneça uma representação JSON do objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="7ac4a-128">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="7ac4a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="7ac4a-129">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="7ac4a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ac4a-130">Property</span></span>|<span data-ttu-id="7ac4a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ac4a-131">Type</span></span>|<span data-ttu-id="7ac4a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ac4a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ac4a-133">id</span><span class="sxs-lookup"><span data-stu-id="7ac4a-133">id</span></span>|<span data-ttu-id="7ac4a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac4a-134">String</span></span>|<span data-ttu-id="7ac4a-135">O identificador exclusivo do parceiro.</span><span class="sxs-lookup"><span data-stu-id="7ac4a-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="7ac4a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7ac4a-136">displayName</span></span>|<span data-ttu-id="7ac4a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac4a-137">String</span></span>|<span data-ttu-id="7ac4a-138">Nome de exibição do parceiro.</span><span class="sxs-lookup"><span data-stu-id="7ac4a-138">Display name of the partner.</span></span>|
|<span data-ttu-id="7ac4a-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="7ac4a-139">onboardingUrl</span></span>|<span data-ttu-id="7ac4a-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac4a-140">String</span></span>|<span data-ttu-id="7ac4a-141">URL do portal de integração do parceiro, no qual um administrador pode configurar o serviço de assistência remota.</span><span class="sxs-lookup"><span data-stu-id="7ac4a-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="7ac4a-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="7ac4a-142">onboardingStatus</span></span>|[<span data-ttu-id="7ac4a-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="7ac4a-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="7ac4a-144">TBD.</span><span class="sxs-lookup"><span data-stu-id="7ac4a-144">TBD.</span></span> <span data-ttu-id="7ac4a-145">Os valores possíveis são: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="7ac4a-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="7ac4a-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="7ac4a-146">lastConnectionDateTime</span></span>|<span data-ttu-id="7ac4a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ac4a-147">DateTimeOffset</span></span>|<span data-ttu-id="7ac4a-148">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="7ac4a-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="7ac4a-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ac4a-149">Response</span></span>
<span data-ttu-id="7ac4a-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ac4a-150">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ac4a-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ac4a-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="7ac4a-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ac4a-152">Request</span></span>
<span data-ttu-id="7ac4a-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ac4a-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
Content-type: application/json
Content-length: 204

{
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="7ac4a-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ac4a-154">Response</span></span>
<span data-ttu-id="7ac4a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ac4a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





