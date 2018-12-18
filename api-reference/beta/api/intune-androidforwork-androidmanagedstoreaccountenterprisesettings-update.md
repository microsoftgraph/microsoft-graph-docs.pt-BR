---
title: Atualizar androidManagedStoreAccountEnterpriseSettings
description: Atualize as propriedades de um objeto androidManagedStoreAccountEnterpriseSettings.
author: tfitzmac
ms.openlocfilehash: ee5fda9e9c6ce92cdf44ec878c2c5835ceed2c49
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356025"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="06e0a-103">Atualizar androidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="06e0a-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="06e0a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="06e0a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06e0a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="06e0a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06e0a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="06e0a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06e0a-107">Atualize as propriedades de um objeto [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="06e0a-107">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06e0a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06e0a-108">Prerequisites</span></span>
<span data-ttu-id="06e0a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06e0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06e0a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06e0a-111">Permission type</span></span>|<span data-ttu-id="06e0a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06e0a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06e0a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06e0a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06e0a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06e0a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06e0a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06e0a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06e0a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06e0a-116">Not supported.</span></span>|
|<span data-ttu-id="06e0a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06e0a-117">Application</span></span>|<span data-ttu-id="06e0a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06e0a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06e0a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06e0a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="06e0a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06e0a-120">Request headers</span></span>
|<span data-ttu-id="06e0a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06e0a-121">Header</span></span>|<span data-ttu-id="06e0a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="06e0a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06e0a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="06e0a-123">Authorization</span></span>|<span data-ttu-id="06e0a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06e0a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06e0a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="06e0a-125">Accept</span></span>|<span data-ttu-id="06e0a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06e0a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06e0a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06e0a-127">Request body</span></span>
<span data-ttu-id="06e0a-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="06e0a-128">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="06e0a-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span><span class="sxs-lookup"><span data-stu-id="06e0a-129">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="06e0a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06e0a-130">Property</span></span>|<span data-ttu-id="06e0a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="06e0a-131">Type</span></span>|<span data-ttu-id="06e0a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="06e0a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06e0a-133">id</span><span class="sxs-lookup"><span data-stu-id="06e0a-133">id</span></span>|<span data-ttu-id="06e0a-134">String</span><span class="sxs-lookup"><span data-stu-id="06e0a-134">String</span></span>|<span data-ttu-id="06e0a-135">O Android armazenar identificador de configurações da empresa de conta</span><span class="sxs-lookup"><span data-stu-id="06e0a-135">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="06e0a-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="06e0a-136">bindStatus</span></span>|[<span data-ttu-id="06e0a-137">androidManagedStoreAccountBindStatus</span><span class="sxs-lookup"><span data-stu-id="06e0a-137">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="06e0a-138">Associe o status do inquilino com a API do EMM Google.</span><span class="sxs-lookup"><span data-stu-id="06e0a-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="06e0a-139">Os valores possíveis são: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="06e0a-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="06e0a-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="06e0a-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="06e0a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06e0a-141">DateTimeOffset</span></span>|<span data-ttu-id="06e0a-142">Hora da conclusão da última sincronização do aplicativo</span><span class="sxs-lookup"><span data-stu-id="06e0a-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="06e0a-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="06e0a-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="06e0a-144">androidManagedStoreAccountAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="06e0a-144">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="06e0a-145">Resultado da última sincronização de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06e0a-145">Last application sync result.</span></span> <span data-ttu-id="06e0a-146">Os possíveis valores são: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="06e0a-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="06e0a-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="06e0a-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="06e0a-148">String</span><span class="sxs-lookup"><span data-stu-id="06e0a-148">String</span></span>|<span data-ttu-id="06e0a-149">UPN proprietária que criou a empresa</span><span class="sxs-lookup"><span data-stu-id="06e0a-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="06e0a-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="06e0a-150">ownerOrganizationName</span></span>|<span data-ttu-id="06e0a-151">String</span><span class="sxs-lookup"><span data-stu-id="06e0a-151">String</span></span>|<span data-ttu-id="06e0a-152">Nome da organização usado quando a inclusão Android Enterprise</span><span class="sxs-lookup"><span data-stu-id="06e0a-152">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="06e0a-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06e0a-153">lastModifiedDateTime</span></span>|<span data-ttu-id="06e0a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06e0a-154">DateTimeOffset</span></span>|<span data-ttu-id="06e0a-155">Hora da última modificação para configurações da empresa Android</span><span class="sxs-lookup"><span data-stu-id="06e0a-155">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="06e0a-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="06e0a-156">enrollmentTarget</span></span>|[<span data-ttu-id="06e0a-157">androidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="06e0a-157">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="06e0a-158">Indica quais usuários podem inscrever dispositivos no gerenciamento de dispositivos Android Enterprise.</span><span class="sxs-lookup"><span data-stu-id="06e0a-158">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="06e0a-159">Os valores possíveis são: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="06e0a-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="06e0a-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="06e0a-160">targetGroupIds</span></span>|<span data-ttu-id="06e0a-161">String collection</span><span class="sxs-lookup"><span data-stu-id="06e0a-161">String collection</span></span>|<span data-ttu-id="06e0a-162">Especifica a quais grupos AAD podem registrar dispositivos no gerenciamento de dispositivos do Android for Work se enrollmentTarget estiver definido como 'Direcionado'</span><span class="sxs-lookup"><span data-stu-id="06e0a-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="06e0a-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="06e0a-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="06e0a-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="06e0a-164">Boolean</span></span>|<span data-ttu-id="06e0a-165">Indica se essa conta é flighting para o gerenciamento de proprietário de dispositivo Android com CloudDPC.</span><span class="sxs-lookup"><span data-stu-id="06e0a-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="06e0a-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="06e0a-166">Response</span></span>
<span data-ttu-id="06e0a-167">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06e0a-167">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06e0a-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06e0a-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="06e0a-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06e0a-169">Request</span></span>
<span data-ttu-id="06e0a-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06e0a-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
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

### <a name="response"></a><span data-ttu-id="06e0a-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="06e0a-171">Response</span></span>
<span data-ttu-id="06e0a-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06e0a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

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
  "deviceOwnerManagementEnabled": true
}
```





