---
title: Atualizar vppToken
description: Atualizar as propriedades de um objeto vppToken.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a7fc1ead8c4a7c7c2a2fc6410bde39b0cc2c62de
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34980534"
---
# <a name="update-vpptoken"></a><span data-ttu-id="3fe98-103">Atualizar vppToken</span><span class="sxs-lookup"><span data-stu-id="3fe98-103">Update vppToken</span></span>

> <span data-ttu-id="3fe98-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3fe98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fe98-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3fe98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fe98-106">Atualizar as propriedades de um objeto [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="3fe98-106">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fe98-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3fe98-107">Prerequisites</span></span>
<span data-ttu-id="3fe98-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fe98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fe98-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3fe98-110">Permission type</span></span>|<span data-ttu-id="3fe98-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3fe98-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fe98-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fe98-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3fe98-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fe98-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3fe98-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fe98-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fe98-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fe98-115">Not supported.</span></span>|
|<span data-ttu-id="3fe98-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3fe98-116">Application</span></span>|<span data-ttu-id="3fe98-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fe98-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fe98-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fe98-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="3fe98-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3fe98-119">Request headers</span></span>
|<span data-ttu-id="3fe98-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3fe98-120">Header</span></span>|<span data-ttu-id="3fe98-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3fe98-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fe98-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3fe98-122">Authorization</span></span>|<span data-ttu-id="3fe98-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fe98-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fe98-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3fe98-124">Accept</span></span>|<span data-ttu-id="3fe98-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3fe98-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fe98-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3fe98-126">Request body</span></span>
<span data-ttu-id="3fe98-127">No corpo da solicitação, forneça uma representação JSON do objeto [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="3fe98-127">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="3fe98-128">A tabela a seguir mostra as propriedades que são necessárias ao criar o [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="3fe98-128">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="3fe98-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fe98-129">Property</span></span>|<span data-ttu-id="3fe98-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fe98-130">Type</span></span>|<span data-ttu-id="3fe98-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fe98-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fe98-132">id</span><span class="sxs-lookup"><span data-stu-id="3fe98-132">id</span></span>|<span data-ttu-id="3fe98-133">String</span><span class="sxs-lookup"><span data-stu-id="3fe98-133">String</span></span>|<span data-ttu-id="3fe98-134">Isso é gerado automaticamente quando o appleVolumePurchaseProgramToken é criado.</span><span class="sxs-lookup"><span data-stu-id="3fe98-134">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="3fe98-135">É a Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3fe98-135">It is the Key of the entity.</span></span>|
|<span data-ttu-id="3fe98-136">organizationName</span><span class="sxs-lookup"><span data-stu-id="3fe98-136">organizationName</span></span>|<span data-ttu-id="3fe98-137">String</span><span class="sxs-lookup"><span data-stu-id="3fe98-137">String</span></span>|<span data-ttu-id="3fe98-138">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="3fe98-138">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="3fe98-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="3fe98-139">vppTokenAccountType</span></span>|[<span data-ttu-id="3fe98-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="3fe98-140">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="3fe98-141">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="3fe98-141">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="3fe98-142">Os valores possíveis são: `business` e `education`.</span><span class="sxs-lookup"><span data-stu-id="3fe98-142">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="3fe98-143">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="3fe98-143">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="3fe98-144">appleId</span><span class="sxs-lookup"><span data-stu-id="3fe98-144">appleId</span></span>|<span data-ttu-id="3fe98-145">String</span><span class="sxs-lookup"><span data-stu-id="3fe98-145">String</span></span>|<span data-ttu-id="3fe98-146">O Apple ID associado ao Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3fe98-146">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3fe98-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3fe98-147">expirationDateTime</span></span>|<span data-ttu-id="3fe98-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fe98-148">DateTimeOffset</span></span>|<span data-ttu-id="3fe98-149">A data e hora de expiração do Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3fe98-149">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3fe98-150">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3fe98-150">lastSyncDateTime</span></span>|<span data-ttu-id="3fe98-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fe98-151">DateTimeOffset</span></span>|<span data-ttu-id="3fe98-152">A última vez que uma sincronização de aplicativo foi realizada com o serviço do Apple Volume Purchase Program usando o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3fe98-152">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3fe98-153">token</span><span class="sxs-lookup"><span data-stu-id="3fe98-153">token</span></span>|<span data-ttu-id="3fe98-154">String</span><span class="sxs-lookup"><span data-stu-id="3fe98-154">String</span></span>|<span data-ttu-id="3fe98-155">A cadeia de caracteres do Token do Apple Volume Purchase Program baixada do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3fe98-155">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="3fe98-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3fe98-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3fe98-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fe98-157">DateTimeOffset</span></span>|<span data-ttu-id="3fe98-158">Data e hora da última modificação associada com o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3fe98-158">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3fe98-159">state</span><span class="sxs-lookup"><span data-stu-id="3fe98-159">state</span></span>|[<span data-ttu-id="3fe98-160">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="3fe98-160">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="3fe98-161">Estado atual do Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3fe98-161">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="3fe98-162">Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="3fe98-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="3fe98-163">Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="3fe98-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="3fe98-164">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="3fe98-164">tokenActionResults</span></span>|<span data-ttu-id="3fe98-165">coleção [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3fe98-165">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="3fe98-166">A coleção de status das ações executadas no token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3fe98-166">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3fe98-167">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="3fe98-167">lastSyncStatus</span></span>|[<span data-ttu-id="3fe98-168">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="3fe98-168">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="3fe98-169">Status atual de sincronização da última sincronização de aplicativo que foi feita usando o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3fe98-169">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="3fe98-170">Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="3fe98-170">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="3fe98-171">Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="3fe98-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="3fe98-172">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="3fe98-172">automaticallyUpdateApps</span></span>|<span data-ttu-id="3fe98-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fe98-173">Boolean</span></span>|<span data-ttu-id="3fe98-174">Se os aplicativos para o token VPP serão automaticamente atualizados ou não.</span><span class="sxs-lookup"><span data-stu-id="3fe98-174">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="3fe98-175">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="3fe98-175">countryOrRegion</span></span>|<span data-ttu-id="3fe98-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fe98-176">String</span></span>|<span data-ttu-id="3fe98-177">Se os aplicativos para o token VPP serão automaticamente atualizados ou não.</span><span class="sxs-lookup"><span data-stu-id="3fe98-177">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="3fe98-178">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="3fe98-178">dataSharingConsentGranted</span></span>|<span data-ttu-id="3fe98-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe98-179">Boolean</span></span>|<span data-ttu-id="3fe98-180">Consentimento concedido para compartilhamento de dados com o Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3fe98-180">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="3fe98-181">displayName</span><span class="sxs-lookup"><span data-stu-id="3fe98-181">displayName</span></span>|<span data-ttu-id="3fe98-182">String</span><span class="sxs-lookup"><span data-stu-id="3fe98-182">String</span></span>|<span data-ttu-id="3fe98-183">Um nome amigável de token especificado pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="3fe98-183">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="3fe98-184">LocationName</span><span class="sxs-lookup"><span data-stu-id="3fe98-184">locationName</span></span>|<span data-ttu-id="3fe98-185">String</span><span class="sxs-lookup"><span data-stu-id="3fe98-185">String</span></span>|<span data-ttu-id="3fe98-186">Local do token retornado da Apple VPP.</span><span class="sxs-lookup"><span data-stu-id="3fe98-186">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="3fe98-187">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="3fe98-187">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="3fe98-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe98-188">Boolean</span></span>|<span data-ttu-id="3fe98-189">Consentimento do administrador para permitir o reivindicação de gerenciamento de token de MDM externo.</span><span class="sxs-lookup"><span data-stu-id="3fe98-189">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="3fe98-190">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3fe98-190">roleScopeTagIds</span></span>|<span data-ttu-id="3fe98-191">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fe98-191">String collection</span></span>|<span data-ttu-id="3fe98-192">IDs de marcas de escopo de função atribuídas a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="3fe98-192">Role Scope Tags IDs assigned to this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="3fe98-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fe98-193">Response</span></span>
<span data-ttu-id="3fe98-194">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [vppToken](../resources/intune-onboarding-vpptoken.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fe98-194">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fe98-195">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fe98-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fe98-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3fe98-196">Request</span></span>
<span data-ttu-id="3fe98-197">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fe98-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 1002

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
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
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="3fe98-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fe98-198">Response</span></span>
<span data-ttu-id="3fe98-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3fe98-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1115

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
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





