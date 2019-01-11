---
title: Atualizar androidForWorkSettings
description: Atualizar as propriedades de um objeto de androidForWorkSettings.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b46daa868d240b7ae50c83d708b8bf744e8079be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849760"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="9b89f-103">Atualizar androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="9b89f-103">Update androidForWorkSettings</span></span>

> <span data-ttu-id="9b89f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9b89f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b89f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9b89f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b89f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9b89f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b89f-107">Atualizar as propriedades de um objeto de [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="9b89f-107">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b89f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9b89f-108">Prerequisites</span></span>
<span data-ttu-id="9b89f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b89f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b89f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b89f-111">Permission type</span></span>|<span data-ttu-id="9b89f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9b89f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b89f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b89f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b89f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b89f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b89f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b89f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b89f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b89f-116">Not supported.</span></span>|
|<span data-ttu-id="9b89f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b89f-117">Application</span></span>|<span data-ttu-id="9b89f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b89f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b89f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b89f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="9b89f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b89f-120">Request headers</span></span>
|<span data-ttu-id="9b89f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b89f-121">Header</span></span>|<span data-ttu-id="9b89f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9b89f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b89f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b89f-123">Authorization</span></span>|<span data-ttu-id="9b89f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b89f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b89f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9b89f-125">Accept</span></span>|<span data-ttu-id="9b89f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b89f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b89f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b89f-127">Request body</span></span>
<span data-ttu-id="9b89f-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="9b89f-128">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="9b89f-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="9b89f-129">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="9b89f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b89f-130">Property</span></span>|<span data-ttu-id="9b89f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b89f-131">Type</span></span>|<span data-ttu-id="9b89f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b89f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b89f-133">id</span><span class="sxs-lookup"><span data-stu-id="9b89f-133">id</span></span>|<span data-ttu-id="9b89f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b89f-134">String</span></span>|<span data-ttu-id="9b89f-135">O identificador de configurações do Android for Work</span><span class="sxs-lookup"><span data-stu-id="9b89f-135">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="9b89f-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="9b89f-136">bindStatus</span></span>|[<span data-ttu-id="9b89f-137">androidForWorkBindStatus</span><span class="sxs-lookup"><span data-stu-id="9b89f-137">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="9b89f-138">Associe o status do inquilino com a API do EMM Google.</span><span class="sxs-lookup"><span data-stu-id="9b89f-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="9b89f-139">Os valores possíveis são: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="9b89f-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="9b89f-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9b89f-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="9b89f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b89f-141">DateTimeOffset</span></span>|<span data-ttu-id="9b89f-142">Hora da conclusão da última sincronização do aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b89f-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="9b89f-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="9b89f-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="9b89f-144">androidForWorkSyncStatus</span><span class="sxs-lookup"><span data-stu-id="9b89f-144">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="9b89f-145">Resultado da última sincronização de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9b89f-145">Last application sync result.</span></span> <span data-ttu-id="9b89f-146">Os possíveis valores são: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="9b89f-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="9b89f-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9b89f-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="9b89f-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b89f-148">String</span></span>|<span data-ttu-id="9b89f-149">UPN proprietária que criou a empresa</span><span class="sxs-lookup"><span data-stu-id="9b89f-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="9b89f-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="9b89f-150">ownerOrganizationName</span></span>|<span data-ttu-id="9b89f-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b89f-151">String</span></span>|<span data-ttu-id="9b89f-152">Nome da organização usada ao integrar o Android for Work</span><span class="sxs-lookup"><span data-stu-id="9b89f-152">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="9b89f-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b89f-153">lastModifiedDateTime</span></span>|<span data-ttu-id="9b89f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b89f-154">DateTimeOffset</span></span>|<span data-ttu-id="9b89f-155">Hora da última modificação das configurações do Android for Work</span><span class="sxs-lookup"><span data-stu-id="9b89f-155">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="9b89f-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="9b89f-156">enrollmentTarget</span></span>|[<span data-ttu-id="9b89f-157">androidForWorkEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="9b89f-157">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="9b89f-158">Indica quais usuários podem inscrever dispositivos no Android para gerenciamento de dispositivo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="9b89f-158">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="9b89f-159">Os valores possíveis são: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="9b89f-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="9b89f-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="9b89f-160">targetGroupIds</span></span>|<span data-ttu-id="9b89f-161">String collection</span><span class="sxs-lookup"><span data-stu-id="9b89f-161">String collection</span></span>|<span data-ttu-id="9b89f-162">Especifica a quais grupos AAD podem registrar dispositivos no gerenciamento de dispositivos do Android for Work se enrollmentTarget estiver definido como 'Direcionado'</span><span class="sxs-lookup"><span data-stu-id="9b89f-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="9b89f-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="9b89f-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="9b89f-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="9b89f-164">Boolean</span></span>|<span data-ttu-id="9b89f-165">Indica se essa conta é flighting para o gerenciamento de proprietário de dispositivo Android com CloudDPC.</span><span class="sxs-lookup"><span data-stu-id="9b89f-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="9b89f-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b89f-166">Response</span></span>
<span data-ttu-id="9b89f-167">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b89f-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b89f-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b89f-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b89f-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b89f-169">Request</span></span>
<span data-ttu-id="9b89f-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b89f-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9b89f-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b89f-171">Response</span></span>
<span data-ttu-id="9b89f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b89f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





