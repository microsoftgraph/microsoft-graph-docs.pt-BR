---
title: Criar androidDeviceOwnerEnrollmentProfile
description: Criar um novo objeto androidDeviceOwnerEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c02d06ca269da451112293e833ca2460e95fd3b2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43395992"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="4e9f9-103">Criar androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="4e9f9-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

<span data-ttu-id="4e9f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e9f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e9f9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e9f9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e9f9-107">Criar um novo objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4e9f9-107">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e9f9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4e9f9-108">Prerequisites</span></span>
<span data-ttu-id="4e9f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e9f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e9f9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e9f9-111">Permission type</span></span>|<span data-ttu-id="4e9f9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4e9f9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e9f9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e9f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e9f9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e9f9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4e9f9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e9f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e9f9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-116">Not supported.</span></span>|
|<span data-ttu-id="4e9f9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e9f9-117">Application</span></span>|<span data-ttu-id="4e9f9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e9f9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e9f9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e9f9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="4e9f9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e9f9-120">Request headers</span></span>
|<span data-ttu-id="4e9f9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e9f9-121">Header</span></span>|<span data-ttu-id="4e9f9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4e9f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e9f9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e9f9-123">Authorization</span></span>|<span data-ttu-id="4e9f9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e9f9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4e9f9-125">Accept</span></span>|<span data-ttu-id="4e9f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e9f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e9f9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e9f9-127">Request body</span></span>
<span data-ttu-id="4e9f9-128">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-128">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="4e9f9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-129">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="4e9f9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e9f9-130">Property</span></span>|<span data-ttu-id="4e9f9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e9f9-131">Type</span></span>|<span data-ttu-id="4e9f9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e9f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e9f9-133">accountId</span><span class="sxs-lookup"><span data-stu-id="4e9f9-133">accountId</span></span>|<span data-ttu-id="4e9f9-134">String</span><span class="sxs-lookup"><span data-stu-id="4e9f9-134">String</span></span>|<span data-ttu-id="4e9f9-135">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="4e9f9-136">id</span><span class="sxs-lookup"><span data-stu-id="4e9f9-136">id</span></span>|<span data-ttu-id="4e9f9-137">String</span><span class="sxs-lookup"><span data-stu-id="4e9f9-137">String</span></span>|<span data-ttu-id="4e9f9-138">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="4e9f9-139">displayName</span><span class="sxs-lookup"><span data-stu-id="4e9f9-139">displayName</span></span>|<span data-ttu-id="4e9f9-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e9f9-140">String</span></span>|<span data-ttu-id="4e9f9-141">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="4e9f9-142">description</span><span class="sxs-lookup"><span data-stu-id="4e9f9-142">description</span></span>|<span data-ttu-id="4e9f9-143">String</span><span class="sxs-lookup"><span data-stu-id="4e9f9-143">String</span></span>|<span data-ttu-id="4e9f9-144">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="4e9f9-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e9f9-145">createdDateTime</span></span>|<span data-ttu-id="4e9f9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e9f9-146">DateTimeOffset</span></span>|<span data-ttu-id="4e9f9-147">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="4e9f9-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e9f9-148">lastModifiedDateTime</span></span>|<span data-ttu-id="4e9f9-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e9f9-149">DateTimeOffset</span></span>|<span data-ttu-id="4e9f9-150">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="4e9f9-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="4e9f9-151">tokenValue</span></span>|<span data-ttu-id="4e9f9-152">String</span><span class="sxs-lookup"><span data-stu-id="4e9f9-152">String</span></span>|<span data-ttu-id="4e9f9-153">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="4e9f9-154">Propriedadetokencreationdatetime</span><span class="sxs-lookup"><span data-stu-id="4e9f9-154">tokenCreationDateTime</span></span>|<span data-ttu-id="4e9f9-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e9f9-155">DateTimeOffset</span></span>|<span data-ttu-id="4e9f9-156">Data e hora em que o token criado mais recentemente foi criado.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-156">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="4e9f9-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4e9f9-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="4e9f9-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e9f9-158">DateTimeOffset</span></span>|<span data-ttu-id="4e9f9-159">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="4e9f9-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4e9f9-160">enrolledDeviceCount</span></span>|<span data-ttu-id="4e9f9-161">Int32</span><span class="sxs-lookup"><span data-stu-id="4e9f9-161">Int32</span></span>|<span data-ttu-id="4e9f9-162">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="4e9f9-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="4e9f9-163">qrCodeContent</span></span>|<span data-ttu-id="4e9f9-164">String</span><span class="sxs-lookup"><span data-stu-id="4e9f9-164">String</span></span>|<span data-ttu-id="4e9f9-165">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="4e9f9-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="4e9f9-166">qrCodeImage</span></span>|[<span data-ttu-id="4e9f9-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4e9f9-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4e9f9-168">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-168">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="4e9f9-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4e9f9-169">roleScopeTagIds</span></span>|<span data-ttu-id="4e9f9-170">Coleção String</span><span class="sxs-lookup"><span data-stu-id="4e9f9-170">String collection</span></span>|<span data-ttu-id="4e9f9-171">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="4e9f9-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e9f9-172">Response</span></span>
<span data-ttu-id="4e9f9-173">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-173">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e9f9-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e9f9-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e9f9-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e9f9-175">Request</span></span>
<span data-ttu-id="4e9f9-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
Content-type: application/json
Content-length: 627

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="4e9f9-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e9f9-177">Response</span></span>
<span data-ttu-id="4e9f9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e9f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 799

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
  "displayName": "Display Name value",
  "description": "Description value",
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



