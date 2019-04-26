---
title: Atualizar vppToken
description: Atualizar as propriedades de um objeto vppToken.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff48f683c9ac5a31d115a92856d2870bdd0d870d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561450"
---
# <a name="update-vpptoken"></a><span data-ttu-id="357c3-103">Atualizar vppToken</span><span class="sxs-lookup"><span data-stu-id="357c3-103">Update vppToken</span></span>

> <span data-ttu-id="357c3-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="357c3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="357c3-105">Atualizar as propriedades de um objeto [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="357c3-105">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="357c3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="357c3-106">Prerequisites</span></span>
<span data-ttu-id="357c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="357c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="357c3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="357c3-109">Permission type</span></span>|<span data-ttu-id="357c3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="357c3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="357c3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="357c3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="357c3-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="357c3-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="357c3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="357c3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="357c3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="357c3-114">Not supported.</span></span>|
|<span data-ttu-id="357c3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="357c3-115">Application</span></span>|<span data-ttu-id="357c3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="357c3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="357c3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="357c3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="357c3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="357c3-118">Request headers</span></span>
|<span data-ttu-id="357c3-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="357c3-119">Header</span></span>|<span data-ttu-id="357c3-120">Valor</span><span class="sxs-lookup"><span data-stu-id="357c3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="357c3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="357c3-121">Authorization</span></span>|<span data-ttu-id="357c3-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="357c3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="357c3-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="357c3-123">Accept</span></span>|<span data-ttu-id="357c3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="357c3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="357c3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="357c3-125">Request body</span></span>
<span data-ttu-id="357c3-126">No corpo da solicitação, forneça uma representação JSON do objeto [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="357c3-126">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="357c3-127">A tabela a seguir mostra as propriedades que são necessárias ao criar o [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="357c3-127">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="357c3-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="357c3-128">Property</span></span>|<span data-ttu-id="357c3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="357c3-129">Type</span></span>|<span data-ttu-id="357c3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="357c3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="357c3-131">id</span><span class="sxs-lookup"><span data-stu-id="357c3-131">id</span></span>|<span data-ttu-id="357c3-132">String</span><span class="sxs-lookup"><span data-stu-id="357c3-132">String</span></span>|<span data-ttu-id="357c3-133">Isso é gerado automaticamente quando o appleVolumePurchaseProgramToken é criado.</span><span class="sxs-lookup"><span data-stu-id="357c3-133">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="357c3-134">É a Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="357c3-134">It is the Key of the entity.</span></span>|
|<span data-ttu-id="357c3-135">organizationName</span><span class="sxs-lookup"><span data-stu-id="357c3-135">organizationName</span></span>|<span data-ttu-id="357c3-136">String</span><span class="sxs-lookup"><span data-stu-id="357c3-136">String</span></span>|<span data-ttu-id="357c3-137">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="357c3-137">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="357c3-138">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="357c3-138">vppTokenAccountType</span></span>|[<span data-ttu-id="357c3-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="357c3-139">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="357c3-140">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="357c3-140">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="357c3-141">Os valores possíveis são: `business` e `education`.</span><span class="sxs-lookup"><span data-stu-id="357c3-141">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="357c3-142">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="357c3-142">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="357c3-143">appleId</span><span class="sxs-lookup"><span data-stu-id="357c3-143">appleId</span></span>|<span data-ttu-id="357c3-144">String</span><span class="sxs-lookup"><span data-stu-id="357c3-144">String</span></span>|<span data-ttu-id="357c3-145">O Apple ID associado ao Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="357c3-145">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="357c3-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="357c3-146">expirationDateTime</span></span>|<span data-ttu-id="357c3-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="357c3-147">DateTimeOffset</span></span>|<span data-ttu-id="357c3-148">A data e hora de expiração do Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="357c3-148">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="357c3-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="357c3-149">lastSyncDateTime</span></span>|<span data-ttu-id="357c3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="357c3-150">DateTimeOffset</span></span>|<span data-ttu-id="357c3-151">A última vez que uma sincronização de aplicativo foi realizada com o serviço do Apple Volume Purchase Program usando o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="357c3-151">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="357c3-152">token</span><span class="sxs-lookup"><span data-stu-id="357c3-152">token</span></span>|<span data-ttu-id="357c3-153">String</span><span class="sxs-lookup"><span data-stu-id="357c3-153">String</span></span>|<span data-ttu-id="357c3-154">A cadeia de caracteres do Token do Apple Volume Purchase Program baixada do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="357c3-154">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="357c3-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="357c3-155">lastModifiedDateTime</span></span>|<span data-ttu-id="357c3-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="357c3-156">DateTimeOffset</span></span>|<span data-ttu-id="357c3-157">Data e hora da última modificação associada com o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="357c3-157">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="357c3-158">state</span><span class="sxs-lookup"><span data-stu-id="357c3-158">state</span></span>|[<span data-ttu-id="357c3-159">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="357c3-159">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="357c3-160">Estado atual do Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="357c3-160">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="357c3-161">Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="357c3-161">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="357c3-162">Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="357c3-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="357c3-163">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="357c3-163">lastSyncStatus</span></span>|[<span data-ttu-id="357c3-164">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="357c3-164">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="357c3-165">Status atual de sincronização da última sincronização de aplicativo que foi feita usando o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="357c3-165">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="357c3-166">Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="357c3-166">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="357c3-167">Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="357c3-167">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="357c3-168">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="357c3-168">automaticallyUpdateApps</span></span>|<span data-ttu-id="357c3-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="357c3-169">Boolean</span></span>|<span data-ttu-id="357c3-170">Se os aplicativos para o token VPP serão automaticamente atualizados.</span><span class="sxs-lookup"><span data-stu-id="357c3-170">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="357c3-171">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="357c3-171">countryOrRegion</span></span>|<span data-ttu-id="357c3-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="357c3-172">String</span></span>|<span data-ttu-id="357c3-173">Se os aplicativos para o token VPP serão automaticamente atualizados ou não.</span><span class="sxs-lookup"><span data-stu-id="357c3-173">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="357c3-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="357c3-174">Response</span></span>
<span data-ttu-id="357c3-175">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [vppToken](../resources/intune-onboarding-vpptoken.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="357c3-175">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="357c3-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="357c3-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="357c3-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="357c3-177">Request</span></span>
<span data-ttu-id="357c3-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="357c3-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="357c3-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="357c3-179">Response</span></span>
<span data-ttu-id="357c3-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="357c3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



