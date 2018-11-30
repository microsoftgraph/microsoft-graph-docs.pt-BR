---
title: Atualizar androidForWorkSettings
description: Atualizar as propriedades de um objeto de androidForWorkSettings.
ms.openlocfilehash: 58d47117dd574dd6adf96f0ebeb46768c8c7368b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041023"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="1cf12-103">Atualizar androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="1cf12-103">Update androidForWorkSettings</span></span>

> <span data-ttu-id="1cf12-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1cf12-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cf12-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1cf12-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1cf12-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1cf12-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1cf12-107">Atualizar as propriedades de um objeto de [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="1cf12-107">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1cf12-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1cf12-108">Prerequisites</span></span>
<span data-ttu-id="1cf12-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cf12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cf12-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cf12-111">Permission type</span></span>|<span data-ttu-id="1cf12-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1cf12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cf12-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cf12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1cf12-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cf12-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1cf12-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cf12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cf12-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cf12-116">Not supported.</span></span>|
|<span data-ttu-id="1cf12-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cf12-117">Application</span></span>|<span data-ttu-id="1cf12-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cf12-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cf12-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cf12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="1cf12-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cf12-120">Request headers</span></span>
|<span data-ttu-id="1cf12-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1cf12-121">Header</span></span>|<span data-ttu-id="1cf12-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1cf12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cf12-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cf12-123">Authorization</span></span>|<span data-ttu-id="1cf12-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cf12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cf12-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1cf12-125">Accept</span></span>|<span data-ttu-id="1cf12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1cf12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cf12-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cf12-127">Request body</span></span>
<span data-ttu-id="1cf12-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="1cf12-128">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="1cf12-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="1cf12-129">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="1cf12-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1cf12-130">Property</span></span>|<span data-ttu-id="1cf12-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cf12-131">Type</span></span>|<span data-ttu-id="1cf12-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cf12-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cf12-133">id</span><span class="sxs-lookup"><span data-stu-id="1cf12-133">id</span></span>|<span data-ttu-id="1cf12-134">String</span><span class="sxs-lookup"><span data-stu-id="1cf12-134">String</span></span>|<span data-ttu-id="1cf12-135">O identificador de configurações do Android for Work</span><span class="sxs-lookup"><span data-stu-id="1cf12-135">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="1cf12-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="1cf12-136">bindStatus</span></span>|[<span data-ttu-id="1cf12-137">androidForWorkBindStatus</span><span class="sxs-lookup"><span data-stu-id="1cf12-137">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="1cf12-138">Associe o status do inquilino com a API do EMM Google.</span><span class="sxs-lookup"><span data-stu-id="1cf12-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="1cf12-139">Os valores possíveis são: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="1cf12-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="1cf12-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1cf12-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="1cf12-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cf12-141">DateTimeOffset</span></span>|<span data-ttu-id="1cf12-142">Hora da conclusão da última sincronização do aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cf12-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="1cf12-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="1cf12-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="1cf12-144">androidForWorkSyncStatus</span><span class="sxs-lookup"><span data-stu-id="1cf12-144">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="1cf12-145">Resultado da última sincronização de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1cf12-145">Last application sync result.</span></span> <span data-ttu-id="1cf12-146">Os possíveis valores são: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="1cf12-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="1cf12-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1cf12-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="1cf12-148">String</span><span class="sxs-lookup"><span data-stu-id="1cf12-148">String</span></span>|<span data-ttu-id="1cf12-149">UPN proprietária que criou a empresa</span><span class="sxs-lookup"><span data-stu-id="1cf12-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="1cf12-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="1cf12-150">ownerOrganizationName</span></span>|<span data-ttu-id="1cf12-151">String</span><span class="sxs-lookup"><span data-stu-id="1cf12-151">String</span></span>|<span data-ttu-id="1cf12-152">Nome da organização usada ao integrar o Android for Work</span><span class="sxs-lookup"><span data-stu-id="1cf12-152">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="1cf12-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cf12-153">lastModifiedDateTime</span></span>|<span data-ttu-id="1cf12-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cf12-154">DateTimeOffset</span></span>|<span data-ttu-id="1cf12-155">Hora da última modificação das configurações do Android for Work</span><span class="sxs-lookup"><span data-stu-id="1cf12-155">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="1cf12-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="1cf12-156">enrollmentTarget</span></span>|[<span data-ttu-id="1cf12-157">androidForWorkEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="1cf12-157">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="1cf12-158">Indica quais usuários podem inscrever dispositivos no Android para gerenciamento de dispositivo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1cf12-158">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="1cf12-159">Os valores possíveis são: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="1cf12-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="1cf12-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="1cf12-160">targetGroupIds</span></span>|<span data-ttu-id="1cf12-161">String collection</span><span class="sxs-lookup"><span data-stu-id="1cf12-161">String collection</span></span>|<span data-ttu-id="1cf12-162">Especifica a quais grupos AAD podem registrar dispositivos no gerenciamento de dispositivos do Android for Work se enrollmentTarget estiver definido como 'Direcionado'</span><span class="sxs-lookup"><span data-stu-id="1cf12-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="1cf12-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="1cf12-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="1cf12-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="1cf12-164">Boolean</span></span>|<span data-ttu-id="1cf12-165">Indica se essa conta é flighting para o gerenciamento de proprietário de dispositivo Android com CloudDPC.</span><span class="sxs-lookup"><span data-stu-id="1cf12-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="1cf12-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cf12-166">Response</span></span>
<span data-ttu-id="1cf12-167">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cf12-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cf12-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1cf12-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="1cf12-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cf12-169">Request</span></span>
<span data-ttu-id="1cf12-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cf12-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 458

{
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

### <a name="response"></a><span data-ttu-id="1cf12-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cf12-171">Response</span></span>
<span data-ttu-id="1cf12-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1cf12-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





