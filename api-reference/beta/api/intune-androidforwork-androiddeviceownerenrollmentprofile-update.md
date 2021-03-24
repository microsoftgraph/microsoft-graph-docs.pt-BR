---
title: Atualizar androidDeviceOwnerEnrollmentProfile
description: Atualize as propriedades de um objeto androidDeviceOwnerEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dbf3a50d08e8f211c14f0d8eab8070e310f560c9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144792"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="aefb8-103">Atualizar androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="aefb8-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

<span data-ttu-id="aefb8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aefb8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aefb8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aefb8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aefb8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aefb8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aefb8-107">Atualize as propriedades de [um objeto androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="aefb8-107">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aefb8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aefb8-108">Prerequisites</span></span>
<span data-ttu-id="aefb8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aefb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aefb8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aefb8-111">Permission type</span></span>|<span data-ttu-id="aefb8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aefb8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aefb8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aefb8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aefb8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aefb8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aefb8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aefb8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aefb8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aefb8-116">Not supported.</span></span>|
|<span data-ttu-id="aefb8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aefb8-117">Application</span></span>|<span data-ttu-id="aefb8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aefb8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aefb8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aefb8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="aefb8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aefb8-120">Request headers</span></span>
|<span data-ttu-id="aefb8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aefb8-121">Header</span></span>|<span data-ttu-id="aefb8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aefb8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aefb8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aefb8-123">Authorization</span></span>|<span data-ttu-id="aefb8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aefb8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aefb8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aefb8-125">Accept</span></span>|<span data-ttu-id="aefb8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aefb8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aefb8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aefb8-127">Request body</span></span>
<span data-ttu-id="aefb8-128">No corpo da solicitação, fornece uma representação JSON para o [objeto androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="aefb8-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="aefb8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="aefb8-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="aefb8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aefb8-130">Property</span></span>|<span data-ttu-id="aefb8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aefb8-131">Type</span></span>|<span data-ttu-id="aefb8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aefb8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aefb8-133">accountId</span><span class="sxs-lookup"><span data-stu-id="aefb8-133">accountId</span></span>|<span data-ttu-id="aefb8-134">String</span><span class="sxs-lookup"><span data-stu-id="aefb8-134">String</span></span>|<span data-ttu-id="aefb8-135">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="aefb8-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="aefb8-136">id</span><span class="sxs-lookup"><span data-stu-id="aefb8-136">id</span></span>|<span data-ttu-id="aefb8-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aefb8-137">String</span></span>|<span data-ttu-id="aefb8-138">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="aefb8-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="aefb8-139">displayName</span><span class="sxs-lookup"><span data-stu-id="aefb8-139">displayName</span></span>|<span data-ttu-id="aefb8-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aefb8-140">String</span></span>|<span data-ttu-id="aefb8-141">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="aefb8-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="aefb8-142">descrição</span><span class="sxs-lookup"><span data-stu-id="aefb8-142">description</span></span>|<span data-ttu-id="aefb8-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aefb8-143">String</span></span>|<span data-ttu-id="aefb8-144">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="aefb8-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="aefb8-145">enrollmentMode</span><span class="sxs-lookup"><span data-stu-id="aefb8-145">enrollmentMode</span></span>|[<span data-ttu-id="aefb8-146">androidDeviceOwnerEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="aefb8-146">androidDeviceOwnerEnrollmentMode</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentmode.md)|<span data-ttu-id="aefb8-147">O modo de registro de dispositivos que usam esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="aefb8-147">The enrollment mode of devices that use this enrollment profile.</span></span> <span data-ttu-id="aefb8-148">Os valores possíveis são: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="aefb8-148">Possible values are: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`.</span></span>|
|<span data-ttu-id="aefb8-149">enrollmentTokenType</span><span class="sxs-lookup"><span data-stu-id="aefb8-149">enrollmentTokenType</span></span>|[<span data-ttu-id="aefb8-150">androidDeviceOwnerEnrollmentTokenType</span><span class="sxs-lookup"><span data-stu-id="aefb8-150">androidDeviceOwnerEnrollmentTokenType</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmenttokentype.md)|<span data-ttu-id="aefb8-151">O tipo de token de registro para um perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="aefb8-151">The enrollment token type for an enrollment profile.</span></span> <span data-ttu-id="aefb8-152">Os valores possíveis são: `default` e `corporateOwnedDedicatedDeviceWithAzureADSharedMode`.</span><span class="sxs-lookup"><span data-stu-id="aefb8-152">Possible values are: `default`, `corporateOwnedDedicatedDeviceWithAzureADSharedMode`.</span></span>|
|<span data-ttu-id="aefb8-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aefb8-153">createdDateTime</span></span>|<span data-ttu-id="aefb8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aefb8-154">DateTimeOffset</span></span>|<span data-ttu-id="aefb8-155">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="aefb8-155">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="aefb8-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aefb8-156">lastModifiedDateTime</span></span>|<span data-ttu-id="aefb8-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aefb8-157">DateTimeOffset</span></span>|<span data-ttu-id="aefb8-158">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="aefb8-158">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="aefb8-159">tokenValue</span><span class="sxs-lookup"><span data-stu-id="aefb8-159">tokenValue</span></span>|<span data-ttu-id="aefb8-160">String</span><span class="sxs-lookup"><span data-stu-id="aefb8-160">String</span></span>|<span data-ttu-id="aefb8-161">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="aefb8-161">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="aefb8-162">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="aefb8-162">tokenCreationDateTime</span></span>|<span data-ttu-id="aefb8-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aefb8-163">DateTimeOffset</span></span>|<span data-ttu-id="aefb8-164">Data em que o token criado mais recentemente foi criado.</span><span class="sxs-lookup"><span data-stu-id="aefb8-164">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="aefb8-165">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="aefb8-165">tokenExpirationDateTime</span></span>|<span data-ttu-id="aefb8-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aefb8-166">DateTimeOffset</span></span>|<span data-ttu-id="aefb8-167">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="aefb8-167">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="aefb8-168">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aefb8-168">enrolledDeviceCount</span></span>|<span data-ttu-id="aefb8-169">Int32</span><span class="sxs-lookup"><span data-stu-id="aefb8-169">Int32</span></span>|<span data-ttu-id="aefb8-170">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="aefb8-170">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="aefb8-171">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="aefb8-171">qrCodeContent</span></span>|<span data-ttu-id="aefb8-172">String</span><span class="sxs-lookup"><span data-stu-id="aefb8-172">String</span></span>|<span data-ttu-id="aefb8-173">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="aefb8-173">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="aefb8-174">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="aefb8-174">qrCodeImage</span></span>|[<span data-ttu-id="aefb8-175">mimeContent</span><span class="sxs-lookup"><span data-stu-id="aefb8-175">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="aefb8-176">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="aefb8-176">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="aefb8-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aefb8-177">roleScopeTagIds</span></span>|<span data-ttu-id="aefb8-178">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aefb8-178">String collection</span></span>|<span data-ttu-id="aefb8-179">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="aefb8-179">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="aefb8-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="aefb8-180">Response</span></span>
<span data-ttu-id="aefb8-181">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aefb8-181">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aefb8-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aefb8-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="aefb8-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aefb8-183">Request</span></span>
<span data-ttu-id="aefb8-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aefb8-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
Content-type: application/json
Content-length: 758

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "enrollmentMode": "corporateOwnedFullyManaged",
  "enrollmentTokenType": "corporateOwnedDedicatedDeviceWithAzureADSharedMode",
  "tokenValue": "Token Value value",
  "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="aefb8-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="aefb8-185">Response</span></span>
<span data-ttu-id="aefb8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aefb8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 930

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
  "displayName": "Display Name value",
  "description": "Description value",
  "enrollmentMode": "corporateOwnedFullyManaged",
  "enrollmentTokenType": "corporateOwnedDedicatedDeviceWithAzureADSharedMode",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




