---
title: Criar vppToken
description: Criar um novo objeto vppToken.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 035e7917be4ba7fea7470f03bd5e3273cbdc8776
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135009"
---
# <a name="create-vpptoken"></a><span data-ttu-id="ec69a-103">Criar vppToken</span><span class="sxs-lookup"><span data-stu-id="ec69a-103">Create vppToken</span></span>

<span data-ttu-id="ec69a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec69a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec69a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ec69a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec69a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec69a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec69a-107">Criar um novo objeto [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="ec69a-107">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec69a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ec69a-108">Prerequisites</span></span>
<span data-ttu-id="ec69a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec69a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec69a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec69a-111">Permission type</span></span>|<span data-ttu-id="ec69a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec69a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec69a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec69a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec69a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec69a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ec69a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec69a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec69a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec69a-116">Not supported.</span></span>|
|<span data-ttu-id="ec69a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec69a-117">Application</span></span>|<span data-ttu-id="ec69a-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec69a-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec69a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec69a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="ec69a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec69a-120">Request headers</span></span>
|<span data-ttu-id="ec69a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec69a-121">Header</span></span>|<span data-ttu-id="ec69a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ec69a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec69a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec69a-123">Authorization</span></span>|<span data-ttu-id="ec69a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec69a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec69a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ec69a-125">Accept</span></span>|<span data-ttu-id="ec69a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec69a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec69a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec69a-127">Request body</span></span>
<span data-ttu-id="ec69a-128">No corpo da solicitação, forneça uma representação JSON do objeto vppToken.</span><span class="sxs-lookup"><span data-stu-id="ec69a-128">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="ec69a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o vppToken.</span><span class="sxs-lookup"><span data-stu-id="ec69a-129">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="ec69a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec69a-130">Property</span></span>|<span data-ttu-id="ec69a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec69a-131">Type</span></span>|<span data-ttu-id="ec69a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec69a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec69a-133">id</span><span class="sxs-lookup"><span data-stu-id="ec69a-133">id</span></span>|<span data-ttu-id="ec69a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec69a-134">String</span></span>|<span data-ttu-id="ec69a-135">Isso é gerado automaticamente quando o appleVolumePurchaseProgramToken é criado.</span><span class="sxs-lookup"><span data-stu-id="ec69a-135">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="ec69a-136">É a Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ec69a-136">It is the Key of the entity.</span></span>|
|<span data-ttu-id="ec69a-137">organizationName</span><span class="sxs-lookup"><span data-stu-id="ec69a-137">organizationName</span></span>|<span data-ttu-id="ec69a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec69a-138">String</span></span>|<span data-ttu-id="ec69a-139">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="ec69a-139">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="ec69a-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ec69a-140">vppTokenAccountType</span></span>|[<span data-ttu-id="ec69a-141">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ec69a-141">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="ec69a-142">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="ec69a-142">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="ec69a-143">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="ec69a-143">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="ec69a-144">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="ec69a-144">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="ec69a-145">appleId</span><span class="sxs-lookup"><span data-stu-id="ec69a-145">appleId</span></span>|<span data-ttu-id="ec69a-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec69a-146">String</span></span>|<span data-ttu-id="ec69a-147">O Apple ID associado ao Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ec69a-147">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ec69a-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ec69a-148">expirationDateTime</span></span>|<span data-ttu-id="ec69a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec69a-149">DateTimeOffset</span></span>|<span data-ttu-id="ec69a-150">A data e hora de expiração do Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ec69a-150">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ec69a-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ec69a-151">lastSyncDateTime</span></span>|<span data-ttu-id="ec69a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec69a-152">DateTimeOffset</span></span>|<span data-ttu-id="ec69a-153">A última vez que uma sincronização de aplicativo foi realizada com o serviço do Apple Volume Purchase Program usando o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ec69a-153">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ec69a-154">token</span><span class="sxs-lookup"><span data-stu-id="ec69a-154">token</span></span>|<span data-ttu-id="ec69a-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec69a-155">String</span></span>|<span data-ttu-id="ec69a-156">A cadeia de caracteres do Token do Apple Volume Purchase Program baixada do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ec69a-156">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="ec69a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec69a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ec69a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec69a-158">DateTimeOffset</span></span>|<span data-ttu-id="ec69a-159">Data e hora da última modificação associada com o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ec69a-159">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ec69a-160">state</span><span class="sxs-lookup"><span data-stu-id="ec69a-160">state</span></span>|[<span data-ttu-id="ec69a-161">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="ec69a-161">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="ec69a-162">Estado atual do Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ec69a-162">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="ec69a-163">Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="ec69a-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="ec69a-164">Os possíveis valores são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`, `duplicateLocationId`.</span><span class="sxs-lookup"><span data-stu-id="ec69a-164">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`, `duplicateLocationId`.</span></span>|
|<span data-ttu-id="ec69a-165">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="ec69a-165">tokenActionResults</span></span>|<span data-ttu-id="ec69a-166">[Coleção vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ec69a-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="ec69a-167">A coleção de status das ações executadas no Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="ec69a-167">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ec69a-168">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ec69a-168">lastSyncStatus</span></span>|[<span data-ttu-id="ec69a-169">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ec69a-169">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="ec69a-170">Status atual de sincronização da última sincronização de aplicativo que foi feita usando o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ec69a-170">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="ec69a-171">Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="ec69a-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="ec69a-172">Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="ec69a-172">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="ec69a-173">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="ec69a-173">automaticallyUpdateApps</span></span>|<span data-ttu-id="ec69a-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec69a-174">Boolean</span></span>|<span data-ttu-id="ec69a-175">Se os aplicativos para o token VPP serão automaticamente atualizados ou não.</span><span class="sxs-lookup"><span data-stu-id="ec69a-175">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="ec69a-176">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="ec69a-176">countryOrRegion</span></span>|<span data-ttu-id="ec69a-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec69a-177">String</span></span>|<span data-ttu-id="ec69a-178">Se os aplicativos para o token VPP serão automaticamente atualizados ou não.</span><span class="sxs-lookup"><span data-stu-id="ec69a-178">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="ec69a-179">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="ec69a-179">dataSharingConsentGranted</span></span>|<span data-ttu-id="ec69a-180">Booleano</span><span class="sxs-lookup"><span data-stu-id="ec69a-180">Boolean</span></span>|<span data-ttu-id="ec69a-181">Consentimento concedido para compartilhamento de dados com o Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="ec69a-181">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="ec69a-182">displayName</span><span class="sxs-lookup"><span data-stu-id="ec69a-182">displayName</span></span>|<span data-ttu-id="ec69a-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec69a-183">String</span></span>|<span data-ttu-id="ec69a-184">Um nome amigável de token especificado pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ec69a-184">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="ec69a-185">locationName</span><span class="sxs-lookup"><span data-stu-id="ec69a-185">locationName</span></span>|<span data-ttu-id="ec69a-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec69a-186">String</span></span>|<span data-ttu-id="ec69a-187">Local do token retornado do VPP da Apple.</span><span class="sxs-lookup"><span data-stu-id="ec69a-187">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="ec69a-188">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="ec69a-188">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="ec69a-189">Booleano</span><span class="sxs-lookup"><span data-stu-id="ec69a-189">Boolean</span></span>|<span data-ttu-id="ec69a-190">Consentimento do administrador para permitir o gerenciamento de token de declaração do MDM externo.</span><span class="sxs-lookup"><span data-stu-id="ec69a-190">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="ec69a-191">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ec69a-191">roleScopeTagIds</span></span>|<span data-ttu-id="ec69a-192">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec69a-192">String collection</span></span>|<span data-ttu-id="ec69a-193">IDs de marcas de escopo de função atribuídas a essa entidade.</span><span class="sxs-lookup"><span data-stu-id="ec69a-193">Role Scope Tags IDs assigned to this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="ec69a-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec69a-194">Response</span></span>
<span data-ttu-id="ec69a-195">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec69a-195">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec69a-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec69a-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec69a-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec69a-197">Request</span></span>
<span data-ttu-id="ec69a-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec69a-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ec69a-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec69a-199">Response</span></span>
<span data-ttu-id="ec69a-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec69a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




