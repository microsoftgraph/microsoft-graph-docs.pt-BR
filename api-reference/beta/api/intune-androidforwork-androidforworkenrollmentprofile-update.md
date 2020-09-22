---
title: Atualizar androidForWorkEnrollmentProfile
description: Atualizar as propriedades de um objeto androidForWorkEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3161679c682aed5c991d4a511b3c6f057d600929
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006640"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="8789e-103">Atualizar androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="8789e-103">Update androidForWorkEnrollmentProfile</span></span>

<span data-ttu-id="8789e-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8789e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8789e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8789e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8789e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8789e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8789e-107">Atualizar as propriedades de um objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="8789e-107">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8789e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8789e-108">Prerequisites</span></span>
<span data-ttu-id="8789e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8789e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8789e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8789e-111">Permission type</span></span>|<span data-ttu-id="8789e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8789e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8789e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8789e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8789e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8789e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8789e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8789e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8789e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8789e-116">Not supported.</span></span>|
|<span data-ttu-id="8789e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8789e-117">Application</span></span>|<span data-ttu-id="8789e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8789e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8789e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8789e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="8789e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8789e-120">Request headers</span></span>
|<span data-ttu-id="8789e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8789e-121">Header</span></span>|<span data-ttu-id="8789e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8789e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8789e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8789e-123">Authorization</span></span>|<span data-ttu-id="8789e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8789e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8789e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8789e-125">Accept</span></span>|<span data-ttu-id="8789e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8789e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8789e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8789e-127">Request body</span></span>
<span data-ttu-id="8789e-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="8789e-128">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="8789e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="8789e-129">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="8789e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8789e-130">Property</span></span>|<span data-ttu-id="8789e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8789e-131">Type</span></span>|<span data-ttu-id="8789e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8789e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8789e-133">accountId</span><span class="sxs-lookup"><span data-stu-id="8789e-133">accountId</span></span>|<span data-ttu-id="8789e-134">String</span><span class="sxs-lookup"><span data-stu-id="8789e-134">String</span></span>|<span data-ttu-id="8789e-135">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="8789e-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="8789e-136">id</span><span class="sxs-lookup"><span data-stu-id="8789e-136">id</span></span>|<span data-ttu-id="8789e-137">String</span><span class="sxs-lookup"><span data-stu-id="8789e-137">String</span></span>|<span data-ttu-id="8789e-138">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="8789e-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="8789e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="8789e-139">displayName</span></span>|<span data-ttu-id="8789e-140">String</span><span class="sxs-lookup"><span data-stu-id="8789e-140">String</span></span>|<span data-ttu-id="8789e-141">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="8789e-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="8789e-142">description</span><span class="sxs-lookup"><span data-stu-id="8789e-142">description</span></span>|<span data-ttu-id="8789e-143">String</span><span class="sxs-lookup"><span data-stu-id="8789e-143">String</span></span>|<span data-ttu-id="8789e-144">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="8789e-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="8789e-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8789e-145">createdDateTime</span></span>|<span data-ttu-id="8789e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8789e-146">DateTimeOffset</span></span>|<span data-ttu-id="8789e-147">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="8789e-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="8789e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8789e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="8789e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8789e-149">DateTimeOffset</span></span>|<span data-ttu-id="8789e-150">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="8789e-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="8789e-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="8789e-151">tokenValue</span></span>|<span data-ttu-id="8789e-152">String</span><span class="sxs-lookup"><span data-stu-id="8789e-152">String</span></span>|<span data-ttu-id="8789e-153">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="8789e-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="8789e-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8789e-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="8789e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8789e-155">DateTimeOffset</span></span>|<span data-ttu-id="8789e-156">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="8789e-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="8789e-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8789e-157">enrolledDeviceCount</span></span>|<span data-ttu-id="8789e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8789e-158">Int32</span></span>|<span data-ttu-id="8789e-159">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="8789e-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="8789e-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="8789e-160">qrCodeContent</span></span>|<span data-ttu-id="8789e-161">String</span><span class="sxs-lookup"><span data-stu-id="8789e-161">String</span></span>|<span data-ttu-id="8789e-162">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="8789e-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="8789e-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="8789e-163">qrCodeImage</span></span>|[<span data-ttu-id="8789e-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8789e-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8789e-165">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="8789e-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="8789e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="8789e-166">Response</span></span>
<span data-ttu-id="8789e-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8789e-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8789e-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8789e-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="8789e-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8789e-169">Request</span></span>
<span data-ttu-id="8789e-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8789e-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8789e-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="8789e-171">Response</span></span>
<span data-ttu-id="8789e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8789e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






