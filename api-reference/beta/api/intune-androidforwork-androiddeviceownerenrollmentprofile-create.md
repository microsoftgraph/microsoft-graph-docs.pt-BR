---
title: Criar androidDeviceOwnerEnrollmentProfile
description: Criar um novo objeto androidDeviceOwnerEnrollmentProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 636843deb4151c98aacf63853c975b75ac9bfd67
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815814"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="a276d-103">Criar androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a276d-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="a276d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a276d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a276d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a276d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a276d-106">Criar um novo objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a276d-106">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a276d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a276d-107">Prerequisites</span></span>
<span data-ttu-id="a276d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a276d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a276d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a276d-110">Permission type</span></span>|<span data-ttu-id="a276d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a276d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a276d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a276d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a276d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a276d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a276d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a276d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a276d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a276d-115">Not supported.</span></span>|
|<span data-ttu-id="a276d-116">Application</span><span class="sxs-lookup"><span data-stu-id="a276d-116">Application</span></span>|<span data-ttu-id="a276d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a276d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a276d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a276d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="a276d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a276d-119">Request headers</span></span>
|<span data-ttu-id="a276d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a276d-120">Header</span></span>|<span data-ttu-id="a276d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a276d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a276d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a276d-122">Authorization</span></span>|<span data-ttu-id="a276d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a276d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a276d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a276d-124">Accept</span></span>|<span data-ttu-id="a276d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a276d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a276d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a276d-126">Request body</span></span>
<span data-ttu-id="a276d-127">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="a276d-127">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="a276d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="a276d-128">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="a276d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a276d-129">Property</span></span>|<span data-ttu-id="a276d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a276d-130">Type</span></span>|<span data-ttu-id="a276d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a276d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a276d-132">accountId</span><span class="sxs-lookup"><span data-stu-id="a276d-132">accountId</span></span>|<span data-ttu-id="a276d-133">String</span><span class="sxs-lookup"><span data-stu-id="a276d-133">String</span></span>|<span data-ttu-id="a276d-134">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="a276d-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="a276d-135">id</span><span class="sxs-lookup"><span data-stu-id="a276d-135">id</span></span>|<span data-ttu-id="a276d-136">String</span><span class="sxs-lookup"><span data-stu-id="a276d-136">String</span></span>|<span data-ttu-id="a276d-137">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="a276d-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="a276d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="a276d-138">displayName</span></span>|<span data-ttu-id="a276d-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a276d-139">String</span></span>|<span data-ttu-id="a276d-140">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="a276d-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="a276d-141">description</span><span class="sxs-lookup"><span data-stu-id="a276d-141">description</span></span>|<span data-ttu-id="a276d-142">String</span><span class="sxs-lookup"><span data-stu-id="a276d-142">String</span></span>|<span data-ttu-id="a276d-143">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="a276d-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="a276d-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a276d-144">createdDateTime</span></span>|<span data-ttu-id="a276d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a276d-145">DateTimeOffset</span></span>|<span data-ttu-id="a276d-146">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="a276d-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="a276d-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a276d-147">lastModifiedDateTime</span></span>|<span data-ttu-id="a276d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a276d-148">DateTimeOffset</span></span>|<span data-ttu-id="a276d-149">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="a276d-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="a276d-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="a276d-150">tokenValue</span></span>|<span data-ttu-id="a276d-151">String</span><span class="sxs-lookup"><span data-stu-id="a276d-151">String</span></span>|<span data-ttu-id="a276d-152">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="a276d-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="a276d-153">Propriedadetokencreationdatetime</span><span class="sxs-lookup"><span data-stu-id="a276d-153">tokenCreationDateTime</span></span>|<span data-ttu-id="a276d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a276d-154">DateTimeOffset</span></span>|<span data-ttu-id="a276d-155">Data e hora em que o token criado mais recentemente foi criado.</span><span class="sxs-lookup"><span data-stu-id="a276d-155">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="a276d-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a276d-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="a276d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a276d-157">DateTimeOffset</span></span>|<span data-ttu-id="a276d-158">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="a276d-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="a276d-159">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a276d-159">enrolledDeviceCount</span></span>|<span data-ttu-id="a276d-160">Int32</span><span class="sxs-lookup"><span data-stu-id="a276d-160">Int32</span></span>|<span data-ttu-id="a276d-161">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="a276d-161">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="a276d-162">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="a276d-162">qrCodeContent</span></span>|<span data-ttu-id="a276d-163">String</span><span class="sxs-lookup"><span data-stu-id="a276d-163">String</span></span>|<span data-ttu-id="a276d-164">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="a276d-164">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="a276d-165">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="a276d-165">qrCodeImage</span></span>|[<span data-ttu-id="a276d-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a276d-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a276d-167">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="a276d-167">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="a276d-168">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a276d-168">roleScopeTagIds</span></span>|<span data-ttu-id="a276d-169">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a276d-169">String collection</span></span>|<span data-ttu-id="a276d-170">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a276d-170">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="a276d-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="a276d-171">Response</span></span>
<span data-ttu-id="a276d-172">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a276d-172">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a276d-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a276d-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="a276d-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a276d-174">Request</span></span>
<span data-ttu-id="a276d-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a276d-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a276d-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="a276d-176">Response</span></span>
<span data-ttu-id="a276d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a276d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




