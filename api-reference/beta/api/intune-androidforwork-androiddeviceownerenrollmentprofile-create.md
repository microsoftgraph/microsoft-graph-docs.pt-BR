---
title: Criar androidDeviceOwnerEnrollmentProfile
description: Criar um novo objeto androidDeviceOwnerEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 749dd91fb22fe9465599e6ec32070f3adfb0f5e8
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37174246"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="26144-103">Criar androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="26144-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="26144-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26144-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26144-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26144-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26144-106">Criar um novo objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="26144-106">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26144-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26144-107">Prerequisites</span></span>
<span data-ttu-id="26144-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26144-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26144-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26144-110">Permission type</span></span>|<span data-ttu-id="26144-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="26144-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26144-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26144-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26144-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26144-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26144-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26144-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26144-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26144-115">Not supported.</span></span>|
|<span data-ttu-id="26144-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26144-116">Application</span></span>|<span data-ttu-id="26144-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26144-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26144-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26144-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="26144-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26144-119">Request headers</span></span>
|<span data-ttu-id="26144-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26144-120">Header</span></span>|<span data-ttu-id="26144-121">Valor</span><span class="sxs-lookup"><span data-stu-id="26144-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26144-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="26144-122">Authorization</span></span>|<span data-ttu-id="26144-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26144-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26144-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26144-124">Accept</span></span>|<span data-ttu-id="26144-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26144-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26144-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26144-126">Request body</span></span>
<span data-ttu-id="26144-127">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="26144-127">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="26144-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="26144-128">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="26144-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26144-129">Property</span></span>|<span data-ttu-id="26144-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="26144-130">Type</span></span>|<span data-ttu-id="26144-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="26144-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26144-132">accountId</span><span class="sxs-lookup"><span data-stu-id="26144-132">accountId</span></span>|<span data-ttu-id="26144-133">String</span><span class="sxs-lookup"><span data-stu-id="26144-133">String</span></span>|<span data-ttu-id="26144-134">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="26144-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="26144-135">id</span><span class="sxs-lookup"><span data-stu-id="26144-135">id</span></span>|<span data-ttu-id="26144-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26144-136">String</span></span>|<span data-ttu-id="26144-137">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="26144-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="26144-138">displayName</span><span class="sxs-lookup"><span data-stu-id="26144-138">displayName</span></span>|<span data-ttu-id="26144-139">String</span><span class="sxs-lookup"><span data-stu-id="26144-139">String</span></span>|<span data-ttu-id="26144-140">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="26144-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="26144-141">descrição</span><span class="sxs-lookup"><span data-stu-id="26144-141">description</span></span>|<span data-ttu-id="26144-142">String</span><span class="sxs-lookup"><span data-stu-id="26144-142">String</span></span>|<span data-ttu-id="26144-143">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="26144-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="26144-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26144-144">createdDateTime</span></span>|<span data-ttu-id="26144-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26144-145">DateTimeOffset</span></span>|<span data-ttu-id="26144-146">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="26144-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="26144-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26144-147">lastModifiedDateTime</span></span>|<span data-ttu-id="26144-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26144-148">DateTimeOffset</span></span>|<span data-ttu-id="26144-149">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="26144-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="26144-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="26144-150">tokenValue</span></span>|<span data-ttu-id="26144-151">String</span><span class="sxs-lookup"><span data-stu-id="26144-151">String</span></span>|<span data-ttu-id="26144-152">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="26144-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="26144-153">Propriedadetokencreationdatetime</span><span class="sxs-lookup"><span data-stu-id="26144-153">tokenCreationDateTime</span></span>|<span data-ttu-id="26144-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26144-154">DateTimeOffset</span></span>|<span data-ttu-id="26144-155">Data e hora em que o token criado mais recentemente foi criado.</span><span class="sxs-lookup"><span data-stu-id="26144-155">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="26144-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="26144-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="26144-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26144-157">DateTimeOffset</span></span>|<span data-ttu-id="26144-158">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="26144-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="26144-159">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26144-159">enrolledDeviceCount</span></span>|<span data-ttu-id="26144-160">Int32</span><span class="sxs-lookup"><span data-stu-id="26144-160">Int32</span></span>|<span data-ttu-id="26144-161">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="26144-161">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="26144-162">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="26144-162">qrCodeContent</span></span>|<span data-ttu-id="26144-163">String</span><span class="sxs-lookup"><span data-stu-id="26144-163">String</span></span>|<span data-ttu-id="26144-164">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="26144-164">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="26144-165">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="26144-165">qrCodeImage</span></span>|[<span data-ttu-id="26144-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="26144-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="26144-167">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="26144-167">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="26144-168">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="26144-168">roleScopeTagIds</span></span>|<span data-ttu-id="26144-169">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="26144-169">String collection</span></span>|<span data-ttu-id="26144-170">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="26144-170">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="26144-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="26144-171">Response</span></span>
<span data-ttu-id="26144-172">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26144-172">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26144-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26144-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="26144-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26144-174">Request</span></span>
<span data-ttu-id="26144-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26144-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="26144-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="26144-176">Response</span></span>
<span data-ttu-id="26144-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26144-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




