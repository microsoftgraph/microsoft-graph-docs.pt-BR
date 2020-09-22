---
title: Atualizar vppToken
description: Atualizar as propriedades de um objeto vppToken.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 64b24bf2f93d3ab3c81ea386915eb6215941ba95
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048579"
---
# <a name="update-vpptoken"></a><span data-ttu-id="78804-103">Atualizar vppToken</span><span class="sxs-lookup"><span data-stu-id="78804-103">Update vppToken</span></span>

<span data-ttu-id="78804-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78804-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78804-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78804-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78804-106">Atualizar as propriedades de um objeto [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="78804-106">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78804-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78804-107">Prerequisites</span></span>
<span data-ttu-id="78804-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78804-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78804-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78804-110">Permission type</span></span>|<span data-ttu-id="78804-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="78804-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78804-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78804-112">Delegated (work or school account)</span></span>|<span data-ttu-id="78804-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78804-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="78804-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78804-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78804-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78804-115">Not supported.</span></span>|
|<span data-ttu-id="78804-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78804-116">Application</span></span>|<span data-ttu-id="78804-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78804-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78804-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78804-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="78804-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78804-119">Request headers</span></span>
|<span data-ttu-id="78804-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78804-120">Header</span></span>|<span data-ttu-id="78804-121">Valor</span><span class="sxs-lookup"><span data-stu-id="78804-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78804-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="78804-122">Authorization</span></span>|<span data-ttu-id="78804-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78804-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78804-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78804-124">Accept</span></span>|<span data-ttu-id="78804-125">application/json</span><span class="sxs-lookup"><span data-stu-id="78804-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78804-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78804-126">Request body</span></span>
<span data-ttu-id="78804-127">No corpo da solicitação, forneça uma representação JSON do objeto [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="78804-127">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="78804-128">A tabela a seguir mostra as propriedades que são necessárias ao criar o [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="78804-128">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="78804-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78804-129">Property</span></span>|<span data-ttu-id="78804-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="78804-130">Type</span></span>|<span data-ttu-id="78804-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="78804-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78804-132">id</span><span class="sxs-lookup"><span data-stu-id="78804-132">id</span></span>|<span data-ttu-id="78804-133">String</span><span class="sxs-lookup"><span data-stu-id="78804-133">String</span></span>|<span data-ttu-id="78804-134">Isso é gerado automaticamente quando o appleVolumePurchaseProgramToken é criado.</span><span class="sxs-lookup"><span data-stu-id="78804-134">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="78804-135">É a Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="78804-135">It is the Key of the entity.</span></span>|
|<span data-ttu-id="78804-136">organizationName</span><span class="sxs-lookup"><span data-stu-id="78804-136">organizationName</span></span>|<span data-ttu-id="78804-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78804-137">String</span></span>|<span data-ttu-id="78804-138">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="78804-138">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="78804-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="78804-139">vppTokenAccountType</span></span>|[<span data-ttu-id="78804-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="78804-140">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="78804-141">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="78804-141">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="78804-142">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="78804-142">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="78804-143">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="78804-143">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="78804-144">appleId</span><span class="sxs-lookup"><span data-stu-id="78804-144">appleId</span></span>|<span data-ttu-id="78804-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78804-145">String</span></span>|<span data-ttu-id="78804-146">O Apple ID associado ao Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="78804-146">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="78804-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="78804-147">expirationDateTime</span></span>|<span data-ttu-id="78804-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78804-148">DateTimeOffset</span></span>|<span data-ttu-id="78804-149">A data e hora de expiração do Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="78804-149">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="78804-150">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="78804-150">lastSyncDateTime</span></span>|<span data-ttu-id="78804-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78804-151">DateTimeOffset</span></span>|<span data-ttu-id="78804-152">A última vez que uma sincronização de aplicativo foi realizada com o serviço do Apple Volume Purchase Program usando o token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="78804-152">The last time when an application sync was done with the Apple volume purchase program service using the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="78804-153">token</span><span class="sxs-lookup"><span data-stu-id="78804-153">token</span></span>|<span data-ttu-id="78804-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78804-154">String</span></span>|<span data-ttu-id="78804-155">A cadeia de caracteres do Token do Apple Volume Purchase Program baixada do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="78804-155">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="78804-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78804-156">lastModifiedDateTime</span></span>|<span data-ttu-id="78804-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78804-157">DateTimeOffset</span></span>|<span data-ttu-id="78804-158">Data e hora da última modificação associada com o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="78804-158">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="78804-159">state</span><span class="sxs-lookup"><span data-stu-id="78804-159">state</span></span>|[<span data-ttu-id="78804-160">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="78804-160">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="78804-161">Estado atual do Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="78804-161">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="78804-162">Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="78804-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="78804-163">Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="78804-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="78804-164">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="78804-164">lastSyncStatus</span></span>|[<span data-ttu-id="78804-165">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="78804-165">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="78804-166">Status atual de sincronização da última sincronização de aplicativo que foi feita usando o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="78804-166">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="78804-167">Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="78804-167">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="78804-168">Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="78804-168">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="78804-169">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="78804-169">automaticallyUpdateApps</span></span>|<span data-ttu-id="78804-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="78804-170">Boolean</span></span>|<span data-ttu-id="78804-171">Se os aplicativos para o token VPP serão automaticamente atualizados ou não.</span><span class="sxs-lookup"><span data-stu-id="78804-171">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="78804-172">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="78804-172">countryOrRegion</span></span>|<span data-ttu-id="78804-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78804-173">String</span></span>|<span data-ttu-id="78804-174">Se os aplicativos para o token VPP serão automaticamente atualizados ou não.</span><span class="sxs-lookup"><span data-stu-id="78804-174">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="78804-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="78804-175">Response</span></span>
<span data-ttu-id="78804-176">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [vppToken](../resources/intune-onboarding-vpptoken.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78804-176">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78804-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78804-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="78804-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78804-178">Request</span></span>
<span data-ttu-id="78804-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78804-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 461

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

### <a name="response"></a><span data-ttu-id="78804-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="78804-180">Response</span></span>
<span data-ttu-id="78804-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78804-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

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
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```









