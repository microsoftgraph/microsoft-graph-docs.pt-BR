---
title: Atualizar androidForWorkSettings
description: Atualizar as propriedades de um objeto de androidForWorkSettings.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 65550bc588eb5fb0f4d2f11ac785d458e8821a7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170788"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="f96e7-103">Atualizar androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="f96e7-103">Update androidForWorkSettings</span></span>

> <span data-ttu-id="f96e7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f96e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f96e7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f96e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f96e7-106">Atualizar as propriedades de um objeto de [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="f96e7-106">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f96e7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f96e7-107">Prerequisites</span></span>
<span data-ttu-id="f96e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f96e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f96e7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f96e7-110">Permission type</span></span>|<span data-ttu-id="f96e7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f96e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f96e7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f96e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f96e7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f96e7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f96e7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f96e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f96e7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f96e7-115">Not supported.</span></span>|
|<span data-ttu-id="f96e7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f96e7-116">Application</span></span>|<span data-ttu-id="f96e7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f96e7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f96e7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f96e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="f96e7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f96e7-119">Request headers</span></span>
|<span data-ttu-id="f96e7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f96e7-120">Header</span></span>|<span data-ttu-id="f96e7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f96e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f96e7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f96e7-122">Authorization</span></span>|<span data-ttu-id="f96e7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f96e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f96e7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f96e7-124">Accept</span></span>|<span data-ttu-id="f96e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f96e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f96e7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f96e7-126">Request body</span></span>
<span data-ttu-id="f96e7-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="f96e7-127">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="f96e7-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="f96e7-128">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="f96e7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f96e7-129">Property</span></span>|<span data-ttu-id="f96e7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f96e7-130">Type</span></span>|<span data-ttu-id="f96e7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f96e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f96e7-132">id</span><span class="sxs-lookup"><span data-stu-id="f96e7-132">id</span></span>|<span data-ttu-id="f96e7-133">String</span><span class="sxs-lookup"><span data-stu-id="f96e7-133">String</span></span>|<span data-ttu-id="f96e7-134">O identificador de configurações do Android for Work</span><span class="sxs-lookup"><span data-stu-id="f96e7-134">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="f96e7-135">bindStatus</span><span class="sxs-lookup"><span data-stu-id="f96e7-135">bindStatus</span></span>|[<span data-ttu-id="f96e7-136">androidForWorkBindStatus</span><span class="sxs-lookup"><span data-stu-id="f96e7-136">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="f96e7-137">Vincule o status do locatário à API do Google EMM.</span><span class="sxs-lookup"><span data-stu-id="f96e7-137">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="f96e7-138">Os valores possíveis são: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="f96e7-138">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="f96e7-139">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f96e7-139">lastAppSyncDateTime</span></span>|<span data-ttu-id="f96e7-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f96e7-140">DateTimeOffset</span></span>|<span data-ttu-id="f96e7-141">Hora da conclusão da última sincronização do aplicativo</span><span class="sxs-lookup"><span data-stu-id="f96e7-141">Last completion time for app sync</span></span>|
|<span data-ttu-id="f96e7-142">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="f96e7-142">lastAppSyncStatus</span></span>|[<span data-ttu-id="f96e7-143">androidForWorkSyncStatus</span><span class="sxs-lookup"><span data-stu-id="f96e7-143">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="f96e7-144">Resultado da última sincronização do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f96e7-144">Last application sync result.</span></span> <span data-ttu-id="f96e7-145">Os possíveis valores são: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="f96e7-145">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="f96e7-146">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f96e7-146">ownerUserPrincipalName</span></span>|<span data-ttu-id="f96e7-147">String</span><span class="sxs-lookup"><span data-stu-id="f96e7-147">String</span></span>|<span data-ttu-id="f96e7-148">UPN proprietária que criou a empresa</span><span class="sxs-lookup"><span data-stu-id="f96e7-148">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="f96e7-149">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="f96e7-149">ownerOrganizationName</span></span>|<span data-ttu-id="f96e7-150">String</span><span class="sxs-lookup"><span data-stu-id="f96e7-150">String</span></span>|<span data-ttu-id="f96e7-151">Nome da organização usada ao integrar o Android for Work</span><span class="sxs-lookup"><span data-stu-id="f96e7-151">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="f96e7-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f96e7-152">lastModifiedDateTime</span></span>|<span data-ttu-id="f96e7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f96e7-153">DateTimeOffset</span></span>|<span data-ttu-id="f96e7-154">Hora da última modificação das configurações do Android for Work</span><span class="sxs-lookup"><span data-stu-id="f96e7-154">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="f96e7-155">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="f96e7-155">enrollmentTarget</span></span>|[<span data-ttu-id="f96e7-156">androidForWorkEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="f96e7-156">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="f96e7-157">Indica quais usuários podem registrar dispositivos no Android para gerenciamento de dispositivos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f96e7-157">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="f96e7-158">Os valores possíveis são: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="f96e7-158">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="f96e7-159">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="f96e7-159">targetGroupIds</span></span>|<span data-ttu-id="f96e7-160">String collection</span><span class="sxs-lookup"><span data-stu-id="f96e7-160">String collection</span></span>|<span data-ttu-id="f96e7-161">Especifica a quais grupos AAD podem registrar dispositivos no gerenciamento de dispositivos do Android for Work se enrollmentTarget estiver definido como 'Direcionado'</span><span class="sxs-lookup"><span data-stu-id="f96e7-161">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="f96e7-162">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="f96e7-162">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="f96e7-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="f96e7-163">Boolean</span></span>|<span data-ttu-id="f96e7-164">Indica se esta conta está comprovando o gerenciamento de proprietário do dispositivo Android com o CloudDPC.</span><span class="sxs-lookup"><span data-stu-id="f96e7-164">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="f96e7-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="f96e7-165">Response</span></span>
<span data-ttu-id="f96e7-166">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f96e7-166">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f96e7-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f96e7-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="f96e7-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f96e7-168">Request</span></span>
<span data-ttu-id="f96e7-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f96e7-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f96e7-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="f96e7-170">Response</span></span>
<span data-ttu-id="f96e7-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f96e7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




