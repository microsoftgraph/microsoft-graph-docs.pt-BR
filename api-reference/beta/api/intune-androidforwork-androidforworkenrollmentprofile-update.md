---
title: Atualizar androidForWorkEnrollmentProfile
description: Atualizar as propriedades de um objeto androidForWorkEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bd44462792224f5c1865ac3ee2148861479f0ae
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938913"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="49896-103">Atualizar androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="49896-103">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="49896-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49896-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49896-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49896-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49896-106">Atualizar as propriedades de um objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="49896-106">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49896-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49896-107">Prerequisites</span></span>
<span data-ttu-id="49896-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49896-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49896-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49896-110">Permission type</span></span>|<span data-ttu-id="49896-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49896-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49896-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49896-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49896-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49896-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49896-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49896-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49896-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49896-115">Not supported.</span></span>|
|<span data-ttu-id="49896-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49896-116">Application</span></span>|<span data-ttu-id="49896-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49896-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49896-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49896-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="49896-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49896-119">Request headers</span></span>
|<span data-ttu-id="49896-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49896-120">Header</span></span>|<span data-ttu-id="49896-121">Valor</span><span class="sxs-lookup"><span data-stu-id="49896-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49896-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="49896-122">Authorization</span></span>|<span data-ttu-id="49896-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49896-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49896-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49896-124">Accept</span></span>|<span data-ttu-id="49896-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49896-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49896-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49896-126">Request body</span></span>
<span data-ttu-id="49896-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="49896-127">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="49896-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="49896-128">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="49896-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49896-129">Property</span></span>|<span data-ttu-id="49896-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="49896-130">Type</span></span>|<span data-ttu-id="49896-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="49896-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49896-132">accountId</span><span class="sxs-lookup"><span data-stu-id="49896-132">accountId</span></span>|<span data-ttu-id="49896-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49896-133">String</span></span>|<span data-ttu-id="49896-134">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="49896-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="49896-135">id</span><span class="sxs-lookup"><span data-stu-id="49896-135">id</span></span>|<span data-ttu-id="49896-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49896-136">String</span></span>|<span data-ttu-id="49896-137">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="49896-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="49896-138">displayName</span><span class="sxs-lookup"><span data-stu-id="49896-138">displayName</span></span>|<span data-ttu-id="49896-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49896-139">String</span></span>|<span data-ttu-id="49896-140">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="49896-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="49896-141">description</span><span class="sxs-lookup"><span data-stu-id="49896-141">description</span></span>|<span data-ttu-id="49896-142">String</span><span class="sxs-lookup"><span data-stu-id="49896-142">String</span></span>|<span data-ttu-id="49896-143">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="49896-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="49896-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49896-144">createdDateTime</span></span>|<span data-ttu-id="49896-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49896-145">DateTimeOffset</span></span>|<span data-ttu-id="49896-146">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="49896-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="49896-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49896-147">lastModifiedDateTime</span></span>|<span data-ttu-id="49896-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49896-148">DateTimeOffset</span></span>|<span data-ttu-id="49896-149">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="49896-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="49896-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="49896-150">tokenValue</span></span>|<span data-ttu-id="49896-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49896-151">String</span></span>|<span data-ttu-id="49896-152">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="49896-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="49896-153">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="49896-153">tokenExpirationDateTime</span></span>|<span data-ttu-id="49896-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49896-154">DateTimeOffset</span></span>|<span data-ttu-id="49896-155">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="49896-155">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="49896-156">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="49896-156">enrolledDeviceCount</span></span>|<span data-ttu-id="49896-157">Int32</span><span class="sxs-lookup"><span data-stu-id="49896-157">Int32</span></span>|<span data-ttu-id="49896-158">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="49896-158">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="49896-159">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="49896-159">qrCodeContent</span></span>|<span data-ttu-id="49896-160">String</span><span class="sxs-lookup"><span data-stu-id="49896-160">String</span></span>|<span data-ttu-id="49896-161">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="49896-161">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="49896-162">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="49896-162">qrCodeImage</span></span>|[<span data-ttu-id="49896-163">mimeContent</span><span class="sxs-lookup"><span data-stu-id="49896-163">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="49896-164">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="49896-164">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="49896-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="49896-165">Response</span></span>
<span data-ttu-id="49896-166">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49896-166">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49896-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49896-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="49896-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49896-168">Request</span></span>
<span data-ttu-id="49896-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49896-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
Content-type: application/json
Content-length: 496

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "tokenValue": "Token Value value",
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

### <a name="response"></a><span data-ttu-id="49896-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="49896-170">Response</span></span>
<span data-ttu-id="49896-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49896-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "e6742553-2553-e674-5325-74e6532574e6",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
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




