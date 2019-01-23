---
title: Atualizar androidManagedStoreAccountEnterpriseSettings
description: Atualize as propriedades de um objeto androidManagedStoreAccountEnterpriseSettings.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e57b7965e5393faf9bdb953dc915652772deb14c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398482"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="1726f-103">Atualizar androidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="1726f-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="1726f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="1726f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1726f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1726f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1726f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="1726f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1726f-107">Atualize as propriedades de um objeto [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="1726f-107">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1726f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1726f-108">Prerequisites</span></span>
<span data-ttu-id="1726f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1726f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1726f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1726f-111">Permission type</span></span>|<span data-ttu-id="1726f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1726f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1726f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1726f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1726f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1726f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1726f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1726f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1726f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1726f-116">Not supported.</span></span>|
|<span data-ttu-id="1726f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1726f-117">Application</span></span>|<span data-ttu-id="1726f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1726f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1726f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1726f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="1726f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1726f-120">Request headers</span></span>
|<span data-ttu-id="1726f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1726f-121">Header</span></span>|<span data-ttu-id="1726f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1726f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1726f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1726f-123">Authorization</span></span>|<span data-ttu-id="1726f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1726f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1726f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1726f-125">Accept</span></span>|<span data-ttu-id="1726f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1726f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1726f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1726f-127">Request body</span></span>
<span data-ttu-id="1726f-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="1726f-128">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="1726f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span><span class="sxs-lookup"><span data-stu-id="1726f-129">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="1726f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1726f-130">Property</span></span>|<span data-ttu-id="1726f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1726f-131">Type</span></span>|<span data-ttu-id="1726f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1726f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1726f-133">id</span><span class="sxs-lookup"><span data-stu-id="1726f-133">id</span></span>|<span data-ttu-id="1726f-134">String</span><span class="sxs-lookup"><span data-stu-id="1726f-134">String</span></span>|<span data-ttu-id="1726f-135">O Android armazenar identificador de configurações da empresa de conta</span><span class="sxs-lookup"><span data-stu-id="1726f-135">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="1726f-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="1726f-136">bindStatus</span></span>|[<span data-ttu-id="1726f-137">androidManagedStoreAccountBindStatus</span><span class="sxs-lookup"><span data-stu-id="1726f-137">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="1726f-138">Associe o status do inquilino com a API do EMM Google.</span><span class="sxs-lookup"><span data-stu-id="1726f-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="1726f-139">Os valores possíveis são: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="1726f-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="1726f-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1726f-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="1726f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1726f-141">DateTimeOffset</span></span>|<span data-ttu-id="1726f-142">Hora da conclusão da última sincronização do aplicativo</span><span class="sxs-lookup"><span data-stu-id="1726f-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="1726f-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="1726f-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="1726f-144">androidManagedStoreAccountAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="1726f-144">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="1726f-145">Resultado da última sincronização de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1726f-145">Last application sync result.</span></span> <span data-ttu-id="1726f-146">Os possíveis valores são: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="1726f-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="1726f-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1726f-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="1726f-148">String</span><span class="sxs-lookup"><span data-stu-id="1726f-148">String</span></span>|<span data-ttu-id="1726f-149">UPN proprietária que criou a empresa</span><span class="sxs-lookup"><span data-stu-id="1726f-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="1726f-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="1726f-150">ownerOrganizationName</span></span>|<span data-ttu-id="1726f-151">String</span><span class="sxs-lookup"><span data-stu-id="1726f-151">String</span></span>|<span data-ttu-id="1726f-152">Nome da organização usado quando a inclusão Android Enterprise</span><span class="sxs-lookup"><span data-stu-id="1726f-152">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="1726f-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1726f-153">lastModifiedDateTime</span></span>|<span data-ttu-id="1726f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1726f-154">DateTimeOffset</span></span>|<span data-ttu-id="1726f-155">Hora da última modificação para configurações da empresa Android</span><span class="sxs-lookup"><span data-stu-id="1726f-155">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="1726f-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="1726f-156">enrollmentTarget</span></span>|[<span data-ttu-id="1726f-157">androidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="1726f-157">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="1726f-158">Indica quais usuários podem inscrever dispositivos no gerenciamento de dispositivos Android Enterprise.</span><span class="sxs-lookup"><span data-stu-id="1726f-158">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="1726f-159">Os valores possíveis são: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="1726f-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="1726f-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="1726f-160">targetGroupIds</span></span>|<span data-ttu-id="1726f-161">String collection</span><span class="sxs-lookup"><span data-stu-id="1726f-161">String collection</span></span>|<span data-ttu-id="1726f-162">Especifica a quais grupos AAD podem registrar dispositivos no gerenciamento de dispositivos do Android for Work se enrollmentTarget estiver definido como 'Direcionado'</span><span class="sxs-lookup"><span data-stu-id="1726f-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="1726f-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="1726f-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="1726f-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="1726f-164">Boolean</span></span>|<span data-ttu-id="1726f-165">Indica se essa conta é flighting para o gerenciamento de proprietário de dispositivo Android com CloudDPC.</span><span class="sxs-lookup"><span data-stu-id="1726f-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|
|<span data-ttu-id="1726f-166">companyCodes</span><span class="sxs-lookup"><span data-stu-id="1726f-166">companyCodes</span></span>|<span data-ttu-id="1726f-167">coleção [androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md)</span><span class="sxs-lookup"><span data-stu-id="1726f-167">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) collection</span></span>|<span data-ttu-id="1726f-168">Códigos de empresa para AndroidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="1726f-168">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|
|<span data-ttu-id="1726f-169">androidDeviceOwnerFullyManagedEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="1726f-169">androidDeviceOwnerFullyManagedEnrollmentEnabled</span></span>|<span data-ttu-id="1726f-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="1726f-170">Boolean</span></span>|<span data-ttu-id="1726f-171">Códigos de empresa para AndroidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="1726f-171">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|



## <a name="response"></a><span data-ttu-id="1726f-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="1726f-172">Response</span></span>
<span data-ttu-id="1726f-173">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1726f-173">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1726f-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1726f-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="1726f-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1726f-175">Request</span></span>
<span data-ttu-id="1726f-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1726f-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1726f-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="1726f-177">Response</span></span>
<span data-ttu-id="1726f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1726f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




