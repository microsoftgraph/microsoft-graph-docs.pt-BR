---
title: Atualizar androidForWorkEnrollmentProfile
description: Atualizar as propriedades de um objeto androidForWorkEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1e2011dc33af2450fe5fe63492167973269441c0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144701"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="a6862-103">Atualizar androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a6862-103">Update androidForWorkEnrollmentProfile</span></span>

<span data-ttu-id="a6862-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6862-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6862-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6862-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6862-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6862-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6862-107">Atualizar as propriedades de um objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="a6862-107">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6862-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6862-108">Prerequisites</span></span>
<span data-ttu-id="a6862-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6862-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6862-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6862-111">Permission type</span></span>|<span data-ttu-id="a6862-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6862-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6862-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6862-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6862-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6862-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6862-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6862-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6862-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6862-116">Not supported.</span></span>|
|<span data-ttu-id="a6862-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6862-117">Application</span></span>|<span data-ttu-id="a6862-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6862-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6862-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6862-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="a6862-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6862-120">Request headers</span></span>
|<span data-ttu-id="a6862-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6862-121">Header</span></span>|<span data-ttu-id="a6862-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a6862-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6862-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6862-123">Authorization</span></span>|<span data-ttu-id="a6862-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6862-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6862-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6862-125">Accept</span></span>|<span data-ttu-id="a6862-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6862-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6862-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6862-127">Request body</span></span>
<span data-ttu-id="a6862-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="a6862-128">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="a6862-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="a6862-129">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="a6862-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6862-130">Property</span></span>|<span data-ttu-id="a6862-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6862-131">Type</span></span>|<span data-ttu-id="a6862-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6862-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6862-133">accountId</span><span class="sxs-lookup"><span data-stu-id="a6862-133">accountId</span></span>|<span data-ttu-id="a6862-134">String</span><span class="sxs-lookup"><span data-stu-id="a6862-134">String</span></span>|<span data-ttu-id="a6862-135">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="a6862-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="a6862-136">id</span><span class="sxs-lookup"><span data-stu-id="a6862-136">id</span></span>|<span data-ttu-id="a6862-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6862-137">String</span></span>|<span data-ttu-id="a6862-138">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="a6862-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="a6862-139">displayName</span><span class="sxs-lookup"><span data-stu-id="a6862-139">displayName</span></span>|<span data-ttu-id="a6862-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6862-140">String</span></span>|<span data-ttu-id="a6862-141">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="a6862-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="a6862-142">descrição</span><span class="sxs-lookup"><span data-stu-id="a6862-142">description</span></span>|<span data-ttu-id="a6862-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6862-143">String</span></span>|<span data-ttu-id="a6862-144">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="a6862-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="a6862-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6862-145">createdDateTime</span></span>|<span data-ttu-id="a6862-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6862-146">DateTimeOffset</span></span>|<span data-ttu-id="a6862-147">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="a6862-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="a6862-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6862-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a6862-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6862-149">DateTimeOffset</span></span>|<span data-ttu-id="a6862-150">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="a6862-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="a6862-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="a6862-151">tokenValue</span></span>|<span data-ttu-id="a6862-152">String</span><span class="sxs-lookup"><span data-stu-id="a6862-152">String</span></span>|<span data-ttu-id="a6862-153">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="a6862-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="a6862-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a6862-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="a6862-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6862-155">DateTimeOffset</span></span>|<span data-ttu-id="a6862-156">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="a6862-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="a6862-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a6862-157">enrolledDeviceCount</span></span>|<span data-ttu-id="a6862-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a6862-158">Int32</span></span>|<span data-ttu-id="a6862-159">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="a6862-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="a6862-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="a6862-160">qrCodeContent</span></span>|<span data-ttu-id="a6862-161">String</span><span class="sxs-lookup"><span data-stu-id="a6862-161">String</span></span>|<span data-ttu-id="a6862-162">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="a6862-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="a6862-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="a6862-163">qrCodeImage</span></span>|[<span data-ttu-id="a6862-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a6862-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a6862-165">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="a6862-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="a6862-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6862-166">Response</span></span>
<span data-ttu-id="a6862-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6862-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6862-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6862-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6862-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6862-169">Request</span></span>
<span data-ttu-id="a6862-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6862-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a6862-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6862-171">Response</span></span>
<span data-ttu-id="a6862-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6862-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




