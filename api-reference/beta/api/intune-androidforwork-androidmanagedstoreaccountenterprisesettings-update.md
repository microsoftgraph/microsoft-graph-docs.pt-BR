---
title: Atualizar androidManagedStoreAccountEnterpriseSettings
description: Atualiza as propriedades de um objeto androidManagedStoreAccountEnterpriseSettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b517e2db80bf3e580a21d5117f7a279144e96c1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324963"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="e569c-103">Atualizar androidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="e569c-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="e569c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e569c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e569c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e569c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e569c-106">Atualiza as propriedades de um objeto [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="e569c-106">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e569c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e569c-107">Prerequisites</span></span>
<span data-ttu-id="e569c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e569c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e569c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e569c-110">Permission type</span></span>|<span data-ttu-id="e569c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e569c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e569c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e569c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e569c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e569c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e569c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e569c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e569c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e569c-115">Not supported.</span></span>|
|<span data-ttu-id="e569c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e569c-116">Application</span></span>|<span data-ttu-id="e569c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e569c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e569c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e569c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="e569c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e569c-119">Request headers</span></span>
|<span data-ttu-id="e569c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e569c-120">Header</span></span>|<span data-ttu-id="e569c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e569c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e569c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e569c-122">Authorization</span></span>|<span data-ttu-id="e569c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e569c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e569c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e569c-124">Accept</span></span>|<span data-ttu-id="e569c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e569c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e569c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e569c-126">Request body</span></span>
<span data-ttu-id="e569c-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="e569c-127">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="e569c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span><span class="sxs-lookup"><span data-stu-id="e569c-128">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="e569c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e569c-129">Property</span></span>|<span data-ttu-id="e569c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e569c-130">Type</span></span>|<span data-ttu-id="e569c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e569c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e569c-132">id</span><span class="sxs-lookup"><span data-stu-id="e569c-132">id</span></span>|<span data-ttu-id="e569c-133">String</span><span class="sxs-lookup"><span data-stu-id="e569c-133">String</span></span>|<span data-ttu-id="e569c-134">O identificador de configurações da empresa da conta do repositório Android</span><span class="sxs-lookup"><span data-stu-id="e569c-134">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="e569c-135">bindStatus</span><span class="sxs-lookup"><span data-stu-id="e569c-135">bindStatus</span></span>|[<span data-ttu-id="e569c-136">androidManagedStoreAccountBindStatus</span><span class="sxs-lookup"><span data-stu-id="e569c-136">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="e569c-137">Vincule o status do locatário à API do Google EMM.</span><span class="sxs-lookup"><span data-stu-id="e569c-137">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="e569c-138">Os valores possíveis são: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="e569c-138">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="e569c-139">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e569c-139">lastAppSyncDateTime</span></span>|<span data-ttu-id="e569c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e569c-140">DateTimeOffset</span></span>|<span data-ttu-id="e569c-141">Hora da conclusão da última sincronização do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e569c-141">Last completion time for app sync</span></span>|
|<span data-ttu-id="e569c-142">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="e569c-142">lastAppSyncStatus</span></span>|[<span data-ttu-id="e569c-143">androidManagedStoreAccountAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="e569c-143">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="e569c-144">Resultado da última sincronização do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e569c-144">Last application sync result.</span></span> <span data-ttu-id="e569c-145">Os possíveis valores são: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="e569c-145">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="e569c-146">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e569c-146">ownerUserPrincipalName</span></span>|<span data-ttu-id="e569c-147">String</span><span class="sxs-lookup"><span data-stu-id="e569c-147">String</span></span>|<span data-ttu-id="e569c-148">UPN proprietária que criou a empresa</span><span class="sxs-lookup"><span data-stu-id="e569c-148">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="e569c-149">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="e569c-149">ownerOrganizationName</span></span>|<span data-ttu-id="e569c-150">String</span><span class="sxs-lookup"><span data-stu-id="e569c-150">String</span></span>|<span data-ttu-id="e569c-151">Nome da organização usado na integração do Android Enterprise</span><span class="sxs-lookup"><span data-stu-id="e569c-151">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="e569c-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e569c-152">lastModifiedDateTime</span></span>|<span data-ttu-id="e569c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e569c-153">DateTimeOffset</span></span>|<span data-ttu-id="e569c-154">Hora da última modificação para configurações corporativas do Android</span><span class="sxs-lookup"><span data-stu-id="e569c-154">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="e569c-155">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="e569c-155">enrollmentTarget</span></span>|[<span data-ttu-id="e569c-156">androidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="e569c-156">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="e569c-157">Indica quais usuários podem registrar dispositivos no gerenciamento de dispositivos do Android Enterprise.</span><span class="sxs-lookup"><span data-stu-id="e569c-157">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="e569c-158">Os valores possíveis são: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="e569c-158">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="e569c-159">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="e569c-159">targetGroupIds</span></span>|<span data-ttu-id="e569c-160">String collection</span><span class="sxs-lookup"><span data-stu-id="e569c-160">String collection</span></span>|<span data-ttu-id="e569c-161">Especifica a quais grupos AAD podem registrar dispositivos no gerenciamento de dispositivos do Android for Work se enrollmentTarget estiver definido como 'Direcionado'</span><span class="sxs-lookup"><span data-stu-id="e569c-161">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="e569c-162">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="e569c-162">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="e569c-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="e569c-163">Boolean</span></span>|<span data-ttu-id="e569c-164">Indica se esta conta está comprovando o gerenciamento de proprietário do dispositivo Android com o CloudDPC.</span><span class="sxs-lookup"><span data-stu-id="e569c-164">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|
|<span data-ttu-id="e569c-165">companyCodes</span><span class="sxs-lookup"><span data-stu-id="e569c-165">companyCodes</span></span>|<span data-ttu-id="e569c-166">coleção [androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md)</span><span class="sxs-lookup"><span data-stu-id="e569c-166">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) collection</span></span>|<span data-ttu-id="e569c-167">Códigos da empresa para AndroidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="e569c-167">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|
|<span data-ttu-id="e569c-168">androidDeviceOwnerFullyManagedEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="e569c-168">androidDeviceOwnerFullyManagedEnrollmentEnabled</span></span>|<span data-ttu-id="e569c-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="e569c-169">Boolean</span></span>|<span data-ttu-id="e569c-170">Códigos da empresa para AndroidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="e569c-170">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|



## <a name="response"></a><span data-ttu-id="e569c-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="e569c-171">Response</span></span>
<span data-ttu-id="e569c-172">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e569c-172">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e569c-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e569c-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="e569c-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e569c-174">Request</span></span>
<span data-ttu-id="e569c-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e569c-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
Content-type: application/json
Content-length: 897

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true,
  "companyCodes": [
    {
      "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
      "enrollmentToken": "Enrollment Token value",
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      }
    }
  ],
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="e569c-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="e569c-176">Response</span></span>
<span data-ttu-id="e569c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e569c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1010

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "id": "b71357c9-57c9-b713-c957-13b7c95713b7",
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
  "deviceOwnerManagementEnabled": true,
  "companyCodes": [
    {
      "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
      "enrollmentToken": "Enrollment Token value",
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      }
    }
  ],
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
}
```






