---
title: Criar vppToken
description: Criar um novo objeto vppToken.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 60289db6f698a4a26656c3f10900c0826e46c000
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757965"
---
# <a name="create-vpptoken"></a><span data-ttu-id="d2649-103">Criar vppToken</span><span class="sxs-lookup"><span data-stu-id="d2649-103">Create vppToken</span></span>

<span data-ttu-id="d2649-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2649-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2649-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2649-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2649-106">Criar um novo objeto [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="d2649-106">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2649-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d2649-107">Prerequisites</span></span>
<span data-ttu-id="d2649-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2649-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2649-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2649-110">Permission type</span></span>|<span data-ttu-id="d2649-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2649-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2649-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2649-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2649-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2649-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d2649-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2649-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2649-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2649-115">Not supported.</span></span>|
|<span data-ttu-id="d2649-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2649-116">Application</span></span>|<span data-ttu-id="d2649-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2649-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2649-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2649-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="d2649-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2649-119">Request headers</span></span>
|<span data-ttu-id="d2649-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d2649-120">Header</span></span>|<span data-ttu-id="d2649-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d2649-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2649-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2649-122">Authorization</span></span>|<span data-ttu-id="d2649-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2649-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2649-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d2649-124">Accept</span></span>|<span data-ttu-id="d2649-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2649-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2649-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2649-126">Request body</span></span>
<span data-ttu-id="d2649-127">No corpo da solicitação, forneça uma representação JSON do objeto vppToken.</span><span class="sxs-lookup"><span data-stu-id="d2649-127">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="d2649-128">A tabela a seguir mostra as propriedades que são necessárias ao criar o vppToken.</span><span class="sxs-lookup"><span data-stu-id="d2649-128">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="d2649-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2649-129">Property</span></span>|<span data-ttu-id="d2649-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2649-130">Type</span></span>|<span data-ttu-id="d2649-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2649-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2649-132">id</span><span class="sxs-lookup"><span data-stu-id="d2649-132">id</span></span>|<span data-ttu-id="d2649-133">String</span><span class="sxs-lookup"><span data-stu-id="d2649-133">String</span></span>|<span data-ttu-id="d2649-134">Isso é gerado automaticamente quando o appleVolumePurchaseProgramToken é criado.</span><span class="sxs-lookup"><span data-stu-id="d2649-134">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="d2649-135">É a Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d2649-135">It is the Key of the entity.</span></span>|
|<span data-ttu-id="d2649-136">organizationName</span><span class="sxs-lookup"><span data-stu-id="d2649-136">organizationName</span></span>|<span data-ttu-id="d2649-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2649-137">String</span></span>|<span data-ttu-id="d2649-138">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="d2649-138">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="d2649-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="d2649-139">vppTokenAccountType</span></span>|[<span data-ttu-id="d2649-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="d2649-140">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="d2649-141">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="d2649-141">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="d2649-142">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="d2649-142">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="d2649-143">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="d2649-143">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="d2649-144">appleId</span><span class="sxs-lookup"><span data-stu-id="d2649-144">appleId</span></span>|<span data-ttu-id="d2649-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2649-145">String</span></span>|<span data-ttu-id="d2649-146">O Apple ID associado ao Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d2649-146">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="d2649-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d2649-147">expirationDateTime</span></span>|<span data-ttu-id="d2649-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2649-148">DateTimeOffset</span></span>|<span data-ttu-id="d2649-149">A data e hora de expiração do Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d2649-149">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="d2649-150">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d2649-150">lastSyncDateTime</span></span>|<span data-ttu-id="d2649-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2649-151">DateTimeOffset</span></span>|<span data-ttu-id="d2649-152">A última vez que uma sincronização de aplicativo foi realizada com o serviço do Apple Volume Purchase Program usando o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d2649-152">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="d2649-153">token</span><span class="sxs-lookup"><span data-stu-id="d2649-153">token</span></span>|<span data-ttu-id="d2649-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2649-154">String</span></span>|<span data-ttu-id="d2649-155">A cadeia de caracteres do Token do Apple Volume Purchase Program baixada do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d2649-155">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="d2649-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2649-156">lastModifiedDateTime</span></span>|<span data-ttu-id="d2649-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2649-157">DateTimeOffset</span></span>|<span data-ttu-id="d2649-158">Data e hora da última modificação associada com o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d2649-158">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="d2649-159">state</span><span class="sxs-lookup"><span data-stu-id="d2649-159">state</span></span>|[<span data-ttu-id="d2649-160">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="d2649-160">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="d2649-161">Estado atual do Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d2649-161">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="d2649-162">Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="d2649-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="d2649-163">Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="d2649-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="d2649-164">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="d2649-164">lastSyncStatus</span></span>|[<span data-ttu-id="d2649-165">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="d2649-165">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="d2649-166">Status atual de sincronização da última sincronização de aplicativo que foi feita usando o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d2649-166">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="d2649-167">Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="d2649-167">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="d2649-168">Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="d2649-168">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="d2649-169">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="d2649-169">automaticallyUpdateApps</span></span>|<span data-ttu-id="d2649-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2649-170">Boolean</span></span>|<span data-ttu-id="d2649-171">Se os aplicativos para o token VPP serão automaticamente atualizados ou não.</span><span class="sxs-lookup"><span data-stu-id="d2649-171">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="d2649-172">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="d2649-172">countryOrRegion</span></span>|<span data-ttu-id="d2649-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2649-173">String</span></span>|<span data-ttu-id="d2649-174">Se os aplicativos para o token VPP serão automaticamente atualizados ou não.</span><span class="sxs-lookup"><span data-stu-id="d2649-174">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="d2649-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2649-175">Response</span></span>
<span data-ttu-id="d2649-176">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2649-176">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2649-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2649-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2649-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2649-178">Request</span></span>
<span data-ttu-id="d2649-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2649-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
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

### <a name="response"></a><span data-ttu-id="d2649-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2649-180">Response</span></span>
<span data-ttu-id="d2649-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2649-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




