---
title: Atualizar androidForWorkSettings
description: Atualizar as propriedades de um objeto de androidForWorkSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eee3c5b6072d715467e50e7b7fcbf3bf0e65ffc5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144659"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="680da-103">Atualizar androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="680da-103">Update androidForWorkSettings</span></span>

<span data-ttu-id="680da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="680da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="680da-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="680da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="680da-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="680da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="680da-107">Atualizar as propriedades de um objeto de [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="680da-107">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="680da-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="680da-108">Prerequisites</span></span>
<span data-ttu-id="680da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="680da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="680da-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="680da-111">Permission type</span></span>|<span data-ttu-id="680da-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="680da-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="680da-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="680da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="680da-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="680da-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="680da-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="680da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="680da-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="680da-116">Not supported.</span></span>|
|<span data-ttu-id="680da-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="680da-117">Application</span></span>|<span data-ttu-id="680da-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="680da-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="680da-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="680da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="680da-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="680da-120">Request headers</span></span>
|<span data-ttu-id="680da-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="680da-121">Header</span></span>|<span data-ttu-id="680da-122">Valor</span><span class="sxs-lookup"><span data-stu-id="680da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="680da-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="680da-123">Authorization</span></span>|<span data-ttu-id="680da-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="680da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="680da-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="680da-125">Accept</span></span>|<span data-ttu-id="680da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="680da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="680da-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="680da-127">Request body</span></span>
<span data-ttu-id="680da-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="680da-128">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="680da-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="680da-129">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="680da-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="680da-130">Property</span></span>|<span data-ttu-id="680da-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="680da-131">Type</span></span>|<span data-ttu-id="680da-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="680da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="680da-133">id</span><span class="sxs-lookup"><span data-stu-id="680da-133">id</span></span>|<span data-ttu-id="680da-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="680da-134">String</span></span>|<span data-ttu-id="680da-135">O identificador de configurações do Android for Work</span><span class="sxs-lookup"><span data-stu-id="680da-135">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="680da-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="680da-136">bindStatus</span></span>|[<span data-ttu-id="680da-137">androidForWorkBindStatus</span><span class="sxs-lookup"><span data-stu-id="680da-137">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="680da-138">Vincular o status do locatário à API de EMM do Google.</span><span class="sxs-lookup"><span data-stu-id="680da-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="680da-139">Os valores possíveis são: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="680da-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="680da-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="680da-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="680da-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="680da-141">DateTimeOffset</span></span>|<span data-ttu-id="680da-142">Hora da conclusão da última sincronização do aplicativo</span><span class="sxs-lookup"><span data-stu-id="680da-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="680da-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="680da-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="680da-144">androidForWorkSyncStatus</span><span class="sxs-lookup"><span data-stu-id="680da-144">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="680da-145">Último resultado de sincronização de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="680da-145">Last application sync result.</span></span> <span data-ttu-id="680da-146">Os possíveis valores são: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="680da-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="680da-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="680da-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="680da-148">String</span><span class="sxs-lookup"><span data-stu-id="680da-148">String</span></span>|<span data-ttu-id="680da-149">UPN proprietária que criou a empresa</span><span class="sxs-lookup"><span data-stu-id="680da-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="680da-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="680da-150">ownerOrganizationName</span></span>|<span data-ttu-id="680da-151">String</span><span class="sxs-lookup"><span data-stu-id="680da-151">String</span></span>|<span data-ttu-id="680da-152">Nome da organização usada ao integrar o Android for Work</span><span class="sxs-lookup"><span data-stu-id="680da-152">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="680da-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="680da-153">lastModifiedDateTime</span></span>|<span data-ttu-id="680da-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="680da-154">DateTimeOffset</span></span>|<span data-ttu-id="680da-155">Hora da última modificação das configurações do Android for Work</span><span class="sxs-lookup"><span data-stu-id="680da-155">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="680da-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="680da-156">enrollmentTarget</span></span>|[<span data-ttu-id="680da-157">androidForWorkEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="680da-157">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="680da-158">Indica quais usuários podem registrar dispositivos no gerenciamento de dispositivos Android for Work.</span><span class="sxs-lookup"><span data-stu-id="680da-158">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="680da-159">Os valores possíveis são: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="680da-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="680da-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="680da-160">targetGroupIds</span></span>|<span data-ttu-id="680da-161">String collection</span><span class="sxs-lookup"><span data-stu-id="680da-161">String collection</span></span>|<span data-ttu-id="680da-162">Especifica a quais grupos AAD podem registrar dispositivos no gerenciamento de dispositivos do Android for Work se enrollmentTarget estiver definido como 'Direcionado'</span><span class="sxs-lookup"><span data-stu-id="680da-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="680da-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="680da-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="680da-164">Booleano</span><span class="sxs-lookup"><span data-stu-id="680da-164">Boolean</span></span>|<span data-ttu-id="680da-165">Indica se essa conta está sendo reativada para o Gerenciamento de Proprietários de Dispositivos Android com o CloudDPC.</span><span class="sxs-lookup"><span data-stu-id="680da-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="680da-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="680da-166">Response</span></span>
<span data-ttu-id="680da-167">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="680da-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="680da-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="680da-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="680da-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="680da-169">Request</span></span>
<span data-ttu-id="680da-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="680da-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="680da-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="680da-171">Response</span></span>
<span data-ttu-id="680da-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="680da-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




