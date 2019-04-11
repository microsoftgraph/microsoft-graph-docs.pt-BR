---
title: Atualizar androidDeviceOwnerEnrollmentProfile
description: Atualiza as propriedades de um objeto androidDeviceOwnerEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c287eb139a7f7aa2fbb6ae2cc9662ac952ff7e2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807767"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="e33e3-103">Atualizar androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e33e3-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="e33e3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e33e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e33e3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e33e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e33e3-106">Atualiza as propriedades de um objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e33e3-106">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e33e3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e33e3-107">Prerequisites</span></span>
<span data-ttu-id="e33e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e33e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e33e3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e33e3-110">Permission type</span></span>|<span data-ttu-id="e33e3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e33e3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e33e3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e33e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e33e3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e33e3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e33e3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e33e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e33e3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e33e3-115">Not supported.</span></span>|
|<span data-ttu-id="e33e3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e33e3-116">Application</span></span>|<span data-ttu-id="e33e3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e33e3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e33e3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e33e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="e33e3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e33e3-119">Request headers</span></span>
|<span data-ttu-id="e33e3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e33e3-120">Header</span></span>|<span data-ttu-id="e33e3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e33e3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e33e3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e33e3-122">Authorization</span></span>|<span data-ttu-id="e33e3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e33e3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e33e3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e33e3-124">Accept</span></span>|<span data-ttu-id="e33e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e33e3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e33e3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e33e3-126">Request body</span></span>
<span data-ttu-id="e33e3-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e33e3-127">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="e33e3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e33e3-128">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="e33e3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e33e3-129">Property</span></span>|<span data-ttu-id="e33e3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e33e3-130">Type</span></span>|<span data-ttu-id="e33e3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e33e3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e33e3-132">accountId</span><span class="sxs-lookup"><span data-stu-id="e33e3-132">accountId</span></span>|<span data-ttu-id="e33e3-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e33e3-133">String</span></span>|<span data-ttu-id="e33e3-134">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="e33e3-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="e33e3-135">id</span><span class="sxs-lookup"><span data-stu-id="e33e3-135">id</span></span>|<span data-ttu-id="e33e3-136">String</span><span class="sxs-lookup"><span data-stu-id="e33e3-136">String</span></span>|<span data-ttu-id="e33e3-137">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="e33e3-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="e33e3-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e33e3-138">displayName</span></span>|<span data-ttu-id="e33e3-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e33e3-139">String</span></span>|<span data-ttu-id="e33e3-140">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="e33e3-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="e33e3-141">description</span><span class="sxs-lookup"><span data-stu-id="e33e3-141">description</span></span>|<span data-ttu-id="e33e3-142">String</span><span class="sxs-lookup"><span data-stu-id="e33e3-142">String</span></span>|<span data-ttu-id="e33e3-143">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="e33e3-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="e33e3-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e33e3-144">createdDateTime</span></span>|<span data-ttu-id="e33e3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e33e3-145">DateTimeOffset</span></span>|<span data-ttu-id="e33e3-146">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="e33e3-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="e33e3-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e33e3-147">lastModifiedDateTime</span></span>|<span data-ttu-id="e33e3-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e33e3-148">DateTimeOffset</span></span>|<span data-ttu-id="e33e3-149">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="e33e3-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="e33e3-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="e33e3-150">tokenValue</span></span>|<span data-ttu-id="e33e3-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e33e3-151">String</span></span>|<span data-ttu-id="e33e3-152">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="e33e3-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="e33e3-153">Propriedadetokencreationdatetime</span><span class="sxs-lookup"><span data-stu-id="e33e3-153">tokenCreationDateTime</span></span>|<span data-ttu-id="e33e3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e33e3-154">DateTimeOffset</span></span>|<span data-ttu-id="e33e3-155">Data e hora em que o token criado mais recentemente foi criado.</span><span class="sxs-lookup"><span data-stu-id="e33e3-155">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="e33e3-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e33e3-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="e33e3-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e33e3-157">DateTimeOffset</span></span>|<span data-ttu-id="e33e3-158">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="e33e3-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="e33e3-159">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e33e3-159">enrolledDeviceCount</span></span>|<span data-ttu-id="e33e3-160">Int32</span><span class="sxs-lookup"><span data-stu-id="e33e3-160">Int32</span></span>|<span data-ttu-id="e33e3-161">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="e33e3-161">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="e33e3-162">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="e33e3-162">qrCodeContent</span></span>|<span data-ttu-id="e33e3-163">String</span><span class="sxs-lookup"><span data-stu-id="e33e3-163">String</span></span>|<span data-ttu-id="e33e3-164">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="e33e3-164">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="e33e3-165">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="e33e3-165">qrCodeImage</span></span>|[<span data-ttu-id="e33e3-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e33e3-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e33e3-167">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="e33e3-167">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="e33e3-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="e33e3-168">Response</span></span>
<span data-ttu-id="e33e3-169">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e33e3-169">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e33e3-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e33e3-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="e33e3-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e33e3-171">Request</span></span>
<span data-ttu-id="e33e3-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e33e3-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
Content-type: application/json
Content-length: 565

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
  }
}
```

### <a name="response"></a><span data-ttu-id="e33e3-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="e33e3-173">Response</span></span>
<span data-ttu-id="e33e3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e33e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 737

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
  }
}
```





