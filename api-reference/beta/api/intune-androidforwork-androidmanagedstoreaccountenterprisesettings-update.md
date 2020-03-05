---
title: Atualizar androidManagedStoreAccountEnterpriseSettings
description: Atualiza as propriedades de um objeto androidManagedStoreAccountEnterpriseSettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 19fdc1fc01c08bb9fda7093dc46d4cf2252f563d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446069"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="7f783-103">Atualizar androidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="7f783-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

<span data-ttu-id="7f783-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7f783-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f783-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7f783-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f783-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f783-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f783-107">Atualiza as propriedades de um objeto [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="7f783-107">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f783-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7f783-108">Prerequisites</span></span>
<span data-ttu-id="7f783-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f783-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f783-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f783-111">Permission type</span></span>|<span data-ttu-id="7f783-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7f783-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f783-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f783-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f783-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f783-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f783-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f783-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f783-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f783-116">Not supported.</span></span>|
|<span data-ttu-id="7f783-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f783-117">Application</span></span>|<span data-ttu-id="7f783-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f783-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f783-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f783-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="7f783-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f783-120">Request headers</span></span>
|<span data-ttu-id="7f783-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f783-121">Header</span></span>|<span data-ttu-id="7f783-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7f783-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f783-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f783-123">Authorization</span></span>|<span data-ttu-id="7f783-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f783-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f783-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7f783-125">Accept</span></span>|<span data-ttu-id="7f783-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f783-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f783-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f783-127">Request body</span></span>
<span data-ttu-id="7f783-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="7f783-128">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="7f783-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span><span class="sxs-lookup"><span data-stu-id="7f783-129">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="7f783-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f783-130">Property</span></span>|<span data-ttu-id="7f783-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f783-131">Type</span></span>|<span data-ttu-id="7f783-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f783-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f783-133">id</span><span class="sxs-lookup"><span data-stu-id="7f783-133">id</span></span>|<span data-ttu-id="7f783-134">String</span><span class="sxs-lookup"><span data-stu-id="7f783-134">String</span></span>|<span data-ttu-id="7f783-135">O identificador de configurações da empresa da conta do repositório Android</span><span class="sxs-lookup"><span data-stu-id="7f783-135">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="7f783-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="7f783-136">bindStatus</span></span>|[<span data-ttu-id="7f783-137">androidManagedStoreAccountBindStatus</span><span class="sxs-lookup"><span data-stu-id="7f783-137">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="7f783-138">Vincule o status do locatário à API do Google EMM.</span><span class="sxs-lookup"><span data-stu-id="7f783-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="7f783-139">Os valores possíveis são: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="7f783-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="7f783-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7f783-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="7f783-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f783-141">DateTimeOffset</span></span>|<span data-ttu-id="7f783-142">Hora da conclusão da última sincronização do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f783-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="7f783-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="7f783-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="7f783-144">androidManagedStoreAccountAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="7f783-144">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="7f783-145">Resultado da última sincronização do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f783-145">Last application sync result.</span></span> <span data-ttu-id="7f783-146">Os possíveis valores são: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="7f783-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="7f783-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7f783-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="7f783-148">String</span><span class="sxs-lookup"><span data-stu-id="7f783-148">String</span></span>|<span data-ttu-id="7f783-149">UPN proprietária que criou a empresa</span><span class="sxs-lookup"><span data-stu-id="7f783-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="7f783-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="7f783-150">ownerOrganizationName</span></span>|<span data-ttu-id="7f783-151">String</span><span class="sxs-lookup"><span data-stu-id="7f783-151">String</span></span>|<span data-ttu-id="7f783-152">Nome da organização usado na integração do Android Enterprise</span><span class="sxs-lookup"><span data-stu-id="7f783-152">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="7f783-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f783-153">lastModifiedDateTime</span></span>|<span data-ttu-id="7f783-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f783-154">DateTimeOffset</span></span>|<span data-ttu-id="7f783-155">Hora da última modificação para configurações corporativas do Android</span><span class="sxs-lookup"><span data-stu-id="7f783-155">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="7f783-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="7f783-156">enrollmentTarget</span></span>|[<span data-ttu-id="7f783-157">androidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="7f783-157">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="7f783-158">Indica quais usuários podem registrar dispositivos no gerenciamento de dispositivos do Android Enterprise.</span><span class="sxs-lookup"><span data-stu-id="7f783-158">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="7f783-159">Os valores possíveis são: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="7f783-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="7f783-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="7f783-160">targetGroupIds</span></span>|<span data-ttu-id="7f783-161">String collection</span><span class="sxs-lookup"><span data-stu-id="7f783-161">String collection</span></span>|<span data-ttu-id="7f783-162">Especifica a quais grupos AAD podem registrar dispositivos no gerenciamento de dispositivos do Android for Work se enrollmentTarget estiver definido como 'Direcionado'</span><span class="sxs-lookup"><span data-stu-id="7f783-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="7f783-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="7f783-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="7f783-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f783-164">Boolean</span></span>|<span data-ttu-id="7f783-165">Indica se esta conta está comprovando o gerenciamento de proprietário do dispositivo Android com o CloudDPC.</span><span class="sxs-lookup"><span data-stu-id="7f783-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|
|<span data-ttu-id="7f783-166">companyCodes</span><span class="sxs-lookup"><span data-stu-id="7f783-166">companyCodes</span></span>|<span data-ttu-id="7f783-167">coleção [androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md)</span><span class="sxs-lookup"><span data-stu-id="7f783-167">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) collection</span></span>|<span data-ttu-id="7f783-168">Códigos da empresa para AndroidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="7f783-168">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|
|<span data-ttu-id="7f783-169">androidDeviceOwnerFullyManagedEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="7f783-169">androidDeviceOwnerFullyManagedEnrollmentEnabled</span></span>|<span data-ttu-id="7f783-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f783-170">Boolean</span></span>|<span data-ttu-id="7f783-171">Códigos da empresa para AndroidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="7f783-171">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|



## <a name="response"></a><span data-ttu-id="7f783-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f783-172">Response</span></span>
<span data-ttu-id="7f783-173">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f783-173">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f783-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f783-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f783-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f783-175">Request</span></span>
<span data-ttu-id="7f783-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f783-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7f783-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f783-177">Response</span></span>
<span data-ttu-id="7f783-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f783-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





