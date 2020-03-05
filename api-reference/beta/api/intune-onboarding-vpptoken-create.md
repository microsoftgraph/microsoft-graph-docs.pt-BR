---
title: Criar vppToken
description: Criar um novo objeto vppToken.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5509c267000961acbf519e0b4b2960b4927e6108
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461771"
---
# <a name="create-vpptoken"></a><span data-ttu-id="21040-103">Criar vppToken</span><span class="sxs-lookup"><span data-stu-id="21040-103">Create vppToken</span></span>

<span data-ttu-id="21040-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="21040-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21040-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21040-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21040-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21040-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21040-107">Criar um novo objeto [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="21040-107">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21040-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21040-108">Prerequisites</span></span>
<span data-ttu-id="21040-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21040-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21040-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21040-111">Permission type</span></span>|<span data-ttu-id="21040-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21040-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21040-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21040-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21040-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21040-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="21040-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21040-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21040-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21040-116">Not supported.</span></span>|
|<span data-ttu-id="21040-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21040-117">Application</span></span>|<span data-ttu-id="21040-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21040-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21040-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21040-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="21040-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21040-120">Request headers</span></span>
|<span data-ttu-id="21040-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21040-121">Header</span></span>|<span data-ttu-id="21040-122">Valor</span><span class="sxs-lookup"><span data-stu-id="21040-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21040-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="21040-123">Authorization</span></span>|<span data-ttu-id="21040-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21040-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21040-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21040-125">Accept</span></span>|<span data-ttu-id="21040-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21040-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21040-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21040-127">Request body</span></span>
<span data-ttu-id="21040-128">No corpo da solicitação, forneça uma representação JSON do objeto vppToken.</span><span class="sxs-lookup"><span data-stu-id="21040-128">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="21040-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o vppToken.</span><span class="sxs-lookup"><span data-stu-id="21040-129">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="21040-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21040-130">Property</span></span>|<span data-ttu-id="21040-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="21040-131">Type</span></span>|<span data-ttu-id="21040-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="21040-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21040-133">id</span><span class="sxs-lookup"><span data-stu-id="21040-133">id</span></span>|<span data-ttu-id="21040-134">String</span><span class="sxs-lookup"><span data-stu-id="21040-134">String</span></span>|<span data-ttu-id="21040-135">Isso é gerado automaticamente quando o appleVolumePurchaseProgramToken é criado.</span><span class="sxs-lookup"><span data-stu-id="21040-135">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="21040-136">É a Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="21040-136">It is the Key of the entity.</span></span>|
|<span data-ttu-id="21040-137">organizationName</span><span class="sxs-lookup"><span data-stu-id="21040-137">organizationName</span></span>|<span data-ttu-id="21040-138">String</span><span class="sxs-lookup"><span data-stu-id="21040-138">String</span></span>|<span data-ttu-id="21040-139">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="21040-139">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="21040-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="21040-140">vppTokenAccountType</span></span>|[<span data-ttu-id="21040-141">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="21040-141">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="21040-142">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="21040-142">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="21040-143">Os valores possíveis são: `business` e `education`.</span><span class="sxs-lookup"><span data-stu-id="21040-143">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="21040-144">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="21040-144">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="21040-145">appleId</span><span class="sxs-lookup"><span data-stu-id="21040-145">appleId</span></span>|<span data-ttu-id="21040-146">String</span><span class="sxs-lookup"><span data-stu-id="21040-146">String</span></span>|<span data-ttu-id="21040-147">O Apple ID associado ao Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="21040-147">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="21040-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="21040-148">expirationDateTime</span></span>|<span data-ttu-id="21040-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21040-149">DateTimeOffset</span></span>|<span data-ttu-id="21040-150">A data e hora de expiração do Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="21040-150">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="21040-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="21040-151">lastSyncDateTime</span></span>|<span data-ttu-id="21040-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21040-152">DateTimeOffset</span></span>|<span data-ttu-id="21040-153">A última vez que uma sincronização de aplicativo foi realizada com o serviço do Apple Volume Purchase Program usando o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="21040-153">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="21040-154">token</span><span class="sxs-lookup"><span data-stu-id="21040-154">token</span></span>|<span data-ttu-id="21040-155">String</span><span class="sxs-lookup"><span data-stu-id="21040-155">String</span></span>|<span data-ttu-id="21040-156">A cadeia de caracteres do Token do Apple Volume Purchase Program baixada do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="21040-156">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="21040-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21040-157">lastModifiedDateTime</span></span>|<span data-ttu-id="21040-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21040-158">DateTimeOffset</span></span>|<span data-ttu-id="21040-159">Data e hora da última modificação associada com o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="21040-159">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="21040-160">state</span><span class="sxs-lookup"><span data-stu-id="21040-160">state</span></span>|[<span data-ttu-id="21040-161">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="21040-161">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="21040-162">Estado atual do Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="21040-162">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="21040-163">Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="21040-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="21040-164">Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="21040-164">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="21040-165">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="21040-165">tokenActionResults</span></span>|<span data-ttu-id="21040-166">coleção [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="21040-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="21040-167">A coleção de status das ações executadas no token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="21040-167">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="21040-168">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="21040-168">lastSyncStatus</span></span>|[<span data-ttu-id="21040-169">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="21040-169">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="21040-170">Status atual de sincronização da última sincronização de aplicativo que foi feita usando o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="21040-170">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="21040-171">Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="21040-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="21040-172">Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="21040-172">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="21040-173">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="21040-173">automaticallyUpdateApps</span></span>|<span data-ttu-id="21040-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="21040-174">Boolean</span></span>|<span data-ttu-id="21040-175">Se os aplicativos para o token VPP serão automaticamente atualizados ou não.</span><span class="sxs-lookup"><span data-stu-id="21040-175">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="21040-176">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="21040-176">countryOrRegion</span></span>|<span data-ttu-id="21040-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21040-177">String</span></span>|<span data-ttu-id="21040-178">Se os aplicativos para o token VPP serão automaticamente atualizados ou não.</span><span class="sxs-lookup"><span data-stu-id="21040-178">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="21040-179">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="21040-179">dataSharingConsentGranted</span></span>|<span data-ttu-id="21040-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="21040-180">Boolean</span></span>|<span data-ttu-id="21040-181">Consentimento concedido para compartilhamento de dados com o Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="21040-181">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="21040-182">displayName</span><span class="sxs-lookup"><span data-stu-id="21040-182">displayName</span></span>|<span data-ttu-id="21040-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21040-183">String</span></span>|<span data-ttu-id="21040-184">Um nome amigável de token especificado pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="21040-184">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="21040-185">LocationName</span><span class="sxs-lookup"><span data-stu-id="21040-185">locationName</span></span>|<span data-ttu-id="21040-186">String</span><span class="sxs-lookup"><span data-stu-id="21040-186">String</span></span>|<span data-ttu-id="21040-187">Local do token retornado da Apple VPP.</span><span class="sxs-lookup"><span data-stu-id="21040-187">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="21040-188">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="21040-188">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="21040-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="21040-189">Boolean</span></span>|<span data-ttu-id="21040-190">Consentimento do administrador para permitir o reivindicação de gerenciamento de token de MDM externo.</span><span class="sxs-lookup"><span data-stu-id="21040-190">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="21040-191">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="21040-191">roleScopeTagIds</span></span>|<span data-ttu-id="21040-192">String collection</span><span class="sxs-lookup"><span data-stu-id="21040-192">String collection</span></span>|<span data-ttu-id="21040-193">IDs de marcas de escopo de função atribuídas a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="21040-193">Role Scope Tags IDs assigned to this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="21040-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="21040-194">Response</span></span>
<span data-ttu-id="21040-195">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21040-195">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21040-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21040-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="21040-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21040-197">Request</span></span>
<span data-ttu-id="21040-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21040-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
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

### <a name="response"></a><span data-ttu-id="21040-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="21040-199">Response</span></span>
<span data-ttu-id="21040-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21040-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





