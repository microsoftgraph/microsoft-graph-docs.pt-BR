---
title: Atualizar vppToken
description: Atualizar as propriedades de um objeto de vppToken.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d1e38660c1fa83ced205b0bbcc506303a3968c41
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954143"
---
# <a name="update-vpptoken"></a><span data-ttu-id="16bf1-103">Atualizar vppToken</span><span class="sxs-lookup"><span data-stu-id="16bf1-103">Update vppToken</span></span>

> <span data-ttu-id="16bf1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="16bf1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16bf1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="16bf1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16bf1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="16bf1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16bf1-107">Atualizar as propriedades de um objeto [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="16bf1-107">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16bf1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16bf1-108">Prerequisites</span></span>
<span data-ttu-id="16bf1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16bf1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16bf1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16bf1-111">Permission type</span></span>|<span data-ttu-id="16bf1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16bf1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16bf1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16bf1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16bf1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16bf1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="16bf1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16bf1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16bf1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16bf1-116">Not supported.</span></span>|
|<span data-ttu-id="16bf1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16bf1-117">Application</span></span>|<span data-ttu-id="16bf1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16bf1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16bf1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16bf1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="16bf1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16bf1-120">Request headers</span></span>
|<span data-ttu-id="16bf1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16bf1-121">Header</span></span>|<span data-ttu-id="16bf1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="16bf1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16bf1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="16bf1-123">Authorization</span></span>|<span data-ttu-id="16bf1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16bf1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16bf1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="16bf1-125">Accept</span></span>|<span data-ttu-id="16bf1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16bf1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16bf1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16bf1-127">Request body</span></span>
<span data-ttu-id="16bf1-128">No corpo da solicitação, forneça uma representação JSON do objeto [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="16bf1-128">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="16bf1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="16bf1-129">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="16bf1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16bf1-130">Property</span></span>|<span data-ttu-id="16bf1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="16bf1-131">Type</span></span>|<span data-ttu-id="16bf1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="16bf1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16bf1-133">id</span><span class="sxs-lookup"><span data-stu-id="16bf1-133">id</span></span>|<span data-ttu-id="16bf1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16bf1-134">String</span></span>|<span data-ttu-id="16bf1-135">Isso é gerado automaticamente quando o appleVolumePurchaseProgramToken é criado.</span><span class="sxs-lookup"><span data-stu-id="16bf1-135">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="16bf1-136">É a Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="16bf1-136">It is the Key of the entity.</span></span>|
|<span data-ttu-id="16bf1-137">organizationName</span><span class="sxs-lookup"><span data-stu-id="16bf1-137">organizationName</span></span>|<span data-ttu-id="16bf1-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16bf1-138">String</span></span>|<span data-ttu-id="16bf1-139">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="16bf1-139">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="16bf1-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="16bf1-140">vppTokenAccountType</span></span>|[<span data-ttu-id="16bf1-141">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="16bf1-141">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="16bf1-142">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="16bf1-142">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="16bf1-143">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="16bf1-143">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="16bf1-144">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="16bf1-144">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="16bf1-145">appleId</span><span class="sxs-lookup"><span data-stu-id="16bf1-145">appleId</span></span>|<span data-ttu-id="16bf1-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16bf1-146">String</span></span>|<span data-ttu-id="16bf1-147">O Apple ID associado ao Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="16bf1-147">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="16bf1-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="16bf1-148">expirationDateTime</span></span>|<span data-ttu-id="16bf1-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16bf1-149">DateTimeOffset</span></span>|<span data-ttu-id="16bf1-150">A data e hora de expiração do Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="16bf1-150">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="16bf1-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="16bf1-151">lastSyncDateTime</span></span>|<span data-ttu-id="16bf1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16bf1-152">DateTimeOffset</span></span>|<span data-ttu-id="16bf1-153">A última vez que uma sincronização de aplicativo foi realizada com o serviço do Apple Volume Purchase Program usando Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="16bf1-153">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="16bf1-154">token</span><span class="sxs-lookup"><span data-stu-id="16bf1-154">token</span></span>|<span data-ttu-id="16bf1-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16bf1-155">String</span></span>|<span data-ttu-id="16bf1-156">A cadeia de caracteres do Token do Apple Volume Purchase Program baixada do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="16bf1-156">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="16bf1-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16bf1-157">lastModifiedDateTime</span></span>|<span data-ttu-id="16bf1-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16bf1-158">DateTimeOffset</span></span>|<span data-ttu-id="16bf1-159">Data e hora da última modificação associada com o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="16bf1-159">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="16bf1-160">state</span><span class="sxs-lookup"><span data-stu-id="16bf1-160">state</span></span>|[<span data-ttu-id="16bf1-161">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="16bf1-161">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="16bf1-162">Estado atual do Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="16bf1-162">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="16bf1-163">Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="16bf1-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="16bf1-164">Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="16bf1-164">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="16bf1-165">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="16bf1-165">tokenActionResults</span></span>|<span data-ttu-id="16bf1-166">coleção [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="16bf1-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="16bf1-167">A coleção dos status das ações executadas em Token para programa de compra do Volume Apple.</span><span class="sxs-lookup"><span data-stu-id="16bf1-167">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="16bf1-168">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="16bf1-168">lastSyncStatus</span></span>|[<span data-ttu-id="16bf1-169">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="16bf1-169">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="16bf1-170">Status atual de sincronização da última sincronização de aplicativo que foi feita usando o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="16bf1-170">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="16bf1-171">Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="16bf1-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="16bf1-172">Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="16bf1-172">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="16bf1-173">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="16bf1-173">automaticallyUpdateApps</span></span>|<span data-ttu-id="16bf1-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="16bf1-174">Boolean</span></span>|<span data-ttu-id="16bf1-175">Se os aplicativos para o token VPP serão automaticamente atualizados ou não.</span><span class="sxs-lookup"><span data-stu-id="16bf1-175">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="16bf1-176">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="16bf1-176">countryOrRegion</span></span>|<span data-ttu-id="16bf1-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16bf1-177">String</span></span>|<span data-ttu-id="16bf1-178">Se os aplicativos para o token VPP serão automaticamente atualizados ou não.</span><span class="sxs-lookup"><span data-stu-id="16bf1-178">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="16bf1-179">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="16bf1-179">dataSharingConsentGranted</span></span>|<span data-ttu-id="16bf1-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="16bf1-180">Boolean</span></span>|<span data-ttu-id="16bf1-181">Consentimento concedido para compartilhamento de dados com o programa de compra de Volume do Apple.</span><span class="sxs-lookup"><span data-stu-id="16bf1-181">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="16bf1-182">displayName</span><span class="sxs-lookup"><span data-stu-id="16bf1-182">displayName</span></span>|<span data-ttu-id="16bf1-183">String</span><span class="sxs-lookup"><span data-stu-id="16bf1-183">String</span></span>|<span data-ttu-id="16bf1-184">Um administrador especificado token nome amigável.</span><span class="sxs-lookup"><span data-stu-id="16bf1-184">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="16bf1-185">locationName</span><span class="sxs-lookup"><span data-stu-id="16bf1-185">locationName</span></span>|<span data-ttu-id="16bf1-186">String</span><span class="sxs-lookup"><span data-stu-id="16bf1-186">String</span></span>|<span data-ttu-id="16bf1-187">Localização de token retornada da Apple VPP.</span><span class="sxs-lookup"><span data-stu-id="16bf1-187">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="16bf1-188">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="16bf1-188">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="16bf1-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="16bf1-189">Boolean</span></span>|<span data-ttu-id="16bf1-190">Admin consentir em permitir que reclamam token gerenciamento do MDM externo.</span><span class="sxs-lookup"><span data-stu-id="16bf1-190">Admin consent to allow claiming token management from external MDM.</span></span>|



## <a name="response"></a><span data-ttu-id="16bf1-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="16bf1-191">Response</span></span>
<span data-ttu-id="16bf1-192">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [vppToken](../resources/intune-onboarding-vpptoken.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16bf1-192">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16bf1-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16bf1-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="16bf1-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16bf1-194">Request</span></span>
<span data-ttu-id="16bf1-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16bf1-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 957

{
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true
}
```

### <a name="response"></a><span data-ttu-id="16bf1-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="16bf1-196">Response</span></span>
<span data-ttu-id="16bf1-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16bf1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1053

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true
}
```





