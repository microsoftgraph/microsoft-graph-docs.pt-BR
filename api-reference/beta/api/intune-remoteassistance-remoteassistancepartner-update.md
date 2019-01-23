---
title: Atualizar remoteAssistancePartner
description: Atualizar as propriedades de um objeto remoteAssistancePartner.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 479c70d13bbdedf9021ca954f6ff16b38be6357a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399014"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="7edbe-103">Atualizar remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="7edbe-103">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="7edbe-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7edbe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7edbe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7edbe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7edbe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7edbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7edbe-107">Atualizar as propriedades de um objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="7edbe-107">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7edbe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7edbe-108">Prerequisites</span></span>
<span data-ttu-id="7edbe-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7edbe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7edbe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7edbe-111">Permission type</span></span>|<span data-ttu-id="7edbe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7edbe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7edbe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7edbe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7edbe-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7edbe-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7edbe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7edbe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7edbe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7edbe-116">Not supported.</span></span>|
|<span data-ttu-id="7edbe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7edbe-117">Application</span></span>|<span data-ttu-id="7edbe-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7edbe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7edbe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7edbe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="7edbe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7edbe-120">Request headers</span></span>
|<span data-ttu-id="7edbe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7edbe-121">Header</span></span>|<span data-ttu-id="7edbe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7edbe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7edbe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7edbe-123">Authorization</span></span>|<span data-ttu-id="7edbe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7edbe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7edbe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7edbe-125">Accept</span></span>|<span data-ttu-id="7edbe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7edbe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7edbe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7edbe-127">Request body</span></span>
<span data-ttu-id="7edbe-128">No corpo da solicitação, forneça uma representação JSON do objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="7edbe-128">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="7edbe-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="7edbe-129">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="7edbe-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7edbe-130">Property</span></span>|<span data-ttu-id="7edbe-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7edbe-131">Type</span></span>|<span data-ttu-id="7edbe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7edbe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7edbe-133">id</span><span class="sxs-lookup"><span data-stu-id="7edbe-133">id</span></span>|<span data-ttu-id="7edbe-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7edbe-134">String</span></span>|<span data-ttu-id="7edbe-135">O identificador exclusivo do parceiro.</span><span class="sxs-lookup"><span data-stu-id="7edbe-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="7edbe-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7edbe-136">displayName</span></span>|<span data-ttu-id="7edbe-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7edbe-137">String</span></span>|<span data-ttu-id="7edbe-138">Nome de exibição do parceiro.</span><span class="sxs-lookup"><span data-stu-id="7edbe-138">Display name of the partner.</span></span>|
|<span data-ttu-id="7edbe-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="7edbe-139">onboardingUrl</span></span>|<span data-ttu-id="7edbe-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7edbe-140">String</span></span>|<span data-ttu-id="7edbe-141">URL do portal de integração do parceiro, no qual um administrador pode configurar o serviço de assistência remota.</span><span class="sxs-lookup"><span data-stu-id="7edbe-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="7edbe-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="7edbe-142">onboardingStatus</span></span>|[<span data-ttu-id="7edbe-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="7edbe-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="7edbe-144">TBD.</span><span class="sxs-lookup"><span data-stu-id="7edbe-144">TBD.</span></span> <span data-ttu-id="7edbe-145">Os valores possíveis são: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="7edbe-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="7edbe-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="7edbe-146">lastConnectionDateTime</span></span>|<span data-ttu-id="7edbe-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7edbe-147">DateTimeOffset</span></span>|<span data-ttu-id="7edbe-148">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="7edbe-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="7edbe-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="7edbe-149">Response</span></span>
<span data-ttu-id="7edbe-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7edbe-150">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7edbe-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7edbe-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="7edbe-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7edbe-152">Request</span></span>
<span data-ttu-id="7edbe-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7edbe-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7edbe-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="7edbe-154">Response</span></span>
<span data-ttu-id="7edbe-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7edbe-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




