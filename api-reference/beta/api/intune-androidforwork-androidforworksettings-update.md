---
title: Atualizar androidForWorkSettings
description: Atualizar as propriedades de um objeto de androidForWorkSettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 221678cef82858e37fb2ff143289b5032099e7bb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34965519"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="a9e64-103">Atualizar androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="a9e64-103">Update androidForWorkSettings</span></span>

> <span data-ttu-id="a9e64-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9e64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9e64-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9e64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9e64-106">Atualizar as propriedades de um objeto de [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="a9e64-106">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9e64-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9e64-107">Prerequisites</span></span>
<span data-ttu-id="a9e64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9e64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9e64-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9e64-110">Permission type</span></span>|<span data-ttu-id="a9e64-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a9e64-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9e64-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9e64-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9e64-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9e64-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9e64-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9e64-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9e64-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9e64-115">Not supported.</span></span>|
|<span data-ttu-id="a9e64-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9e64-116">Application</span></span>|<span data-ttu-id="a9e64-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9e64-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9e64-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9e64-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="a9e64-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9e64-119">Request headers</span></span>
|<span data-ttu-id="a9e64-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9e64-120">Header</span></span>|<span data-ttu-id="a9e64-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a9e64-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9e64-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9e64-122">Authorization</span></span>|<span data-ttu-id="a9e64-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9e64-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9e64-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a9e64-124">Accept</span></span>|<span data-ttu-id="a9e64-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9e64-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9e64-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9e64-126">Request body</span></span>
<span data-ttu-id="a9e64-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="a9e64-127">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="a9e64-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="a9e64-128">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="a9e64-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9e64-129">Property</span></span>|<span data-ttu-id="a9e64-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9e64-130">Type</span></span>|<span data-ttu-id="a9e64-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9e64-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9e64-132">id</span><span class="sxs-lookup"><span data-stu-id="a9e64-132">id</span></span>|<span data-ttu-id="a9e64-133">String</span><span class="sxs-lookup"><span data-stu-id="a9e64-133">String</span></span>|<span data-ttu-id="a9e64-134">O identificador de configurações do Android for Work</span><span class="sxs-lookup"><span data-stu-id="a9e64-134">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="a9e64-135">bindStatus</span><span class="sxs-lookup"><span data-stu-id="a9e64-135">bindStatus</span></span>|[<span data-ttu-id="a9e64-136">androidForWorkBindStatus</span><span class="sxs-lookup"><span data-stu-id="a9e64-136">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="a9e64-137">Vincule o status do locatário à API do Google EMM.</span><span class="sxs-lookup"><span data-stu-id="a9e64-137">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="a9e64-138">Os valores possíveis são: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="a9e64-138">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="a9e64-139">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a9e64-139">lastAppSyncDateTime</span></span>|<span data-ttu-id="a9e64-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9e64-140">DateTimeOffset</span></span>|<span data-ttu-id="a9e64-141">Hora da conclusão da última sincronização do aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9e64-141">Last completion time for app sync</span></span>|
|<span data-ttu-id="a9e64-142">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="a9e64-142">lastAppSyncStatus</span></span>|[<span data-ttu-id="a9e64-143">androidForWorkSyncStatus</span><span class="sxs-lookup"><span data-stu-id="a9e64-143">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="a9e64-144">Resultado da última sincronização do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a9e64-144">Last application sync result.</span></span> <span data-ttu-id="a9e64-145">Os possíveis valores são: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="a9e64-145">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="a9e64-146">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a9e64-146">ownerUserPrincipalName</span></span>|<span data-ttu-id="a9e64-147">String</span><span class="sxs-lookup"><span data-stu-id="a9e64-147">String</span></span>|<span data-ttu-id="a9e64-148">UPN proprietária que criou a empresa</span><span class="sxs-lookup"><span data-stu-id="a9e64-148">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="a9e64-149">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="a9e64-149">ownerOrganizationName</span></span>|<span data-ttu-id="a9e64-150">String</span><span class="sxs-lookup"><span data-stu-id="a9e64-150">String</span></span>|<span data-ttu-id="a9e64-151">Nome da organização usada ao integrar o Android for Work</span><span class="sxs-lookup"><span data-stu-id="a9e64-151">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="a9e64-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9e64-152">lastModifiedDateTime</span></span>|<span data-ttu-id="a9e64-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9e64-153">DateTimeOffset</span></span>|<span data-ttu-id="a9e64-154">Hora da última modificação das configurações do Android for Work</span><span class="sxs-lookup"><span data-stu-id="a9e64-154">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="a9e64-155">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="a9e64-155">enrollmentTarget</span></span>|[<span data-ttu-id="a9e64-156">androidForWorkEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="a9e64-156">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="a9e64-157">Indica quais usuários podem registrar dispositivos no Android para gerenciamento de dispositivos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a9e64-157">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="a9e64-158">Os valores possíveis são: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="a9e64-158">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="a9e64-159">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="a9e64-159">targetGroupIds</span></span>|<span data-ttu-id="a9e64-160">String collection</span><span class="sxs-lookup"><span data-stu-id="a9e64-160">String collection</span></span>|<span data-ttu-id="a9e64-161">Especifica a quais grupos AAD podem registrar dispositivos no gerenciamento de dispositivos do Android for Work se enrollmentTarget estiver definido como 'Direcionado'</span><span class="sxs-lookup"><span data-stu-id="a9e64-161">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="a9e64-162">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="a9e64-162">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="a9e64-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9e64-163">Boolean</span></span>|<span data-ttu-id="a9e64-164">Indica se esta conta está comprovando o gerenciamento de proprietário do dispositivo Android com o CloudDPC.</span><span class="sxs-lookup"><span data-stu-id="a9e64-164">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="a9e64-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9e64-165">Response</span></span>
<span data-ttu-id="a9e64-166">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9e64-166">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9e64-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9e64-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9e64-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9e64-168">Request</span></span>
<span data-ttu-id="a9e64-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9e64-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="a9e64-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9e64-170">Response</span></span>
<span data-ttu-id="a9e64-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9e64-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 568

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```





