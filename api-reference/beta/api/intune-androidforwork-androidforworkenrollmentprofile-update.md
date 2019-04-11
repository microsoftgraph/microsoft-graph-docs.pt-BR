---
title: Atualizar androidForWorkEnrollmentProfile
description: Atualizar as propriedades de um objeto androidForWorkEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2bbb90bda3e9e3306fc71be5ce38d6605f0d306
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776882"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="21715-103">Atualizar androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="21715-103">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="21715-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21715-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21715-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21715-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21715-106">Atualizar as propriedades de um objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="21715-106">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21715-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21715-107">Prerequisites</span></span>
<span data-ttu-id="21715-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21715-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21715-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21715-110">Permission type</span></span>|<span data-ttu-id="21715-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21715-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21715-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21715-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21715-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21715-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="21715-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21715-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21715-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21715-115">Not supported.</span></span>|
|<span data-ttu-id="21715-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21715-116">Application</span></span>|<span data-ttu-id="21715-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21715-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21715-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21715-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="21715-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21715-119">Request headers</span></span>
|<span data-ttu-id="21715-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21715-120">Header</span></span>|<span data-ttu-id="21715-121">Valor</span><span class="sxs-lookup"><span data-stu-id="21715-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21715-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="21715-122">Authorization</span></span>|<span data-ttu-id="21715-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21715-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21715-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21715-124">Accept</span></span>|<span data-ttu-id="21715-125">application/json</span><span class="sxs-lookup"><span data-stu-id="21715-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21715-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21715-126">Request body</span></span>
<span data-ttu-id="21715-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="21715-127">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="21715-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="21715-128">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="21715-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21715-129">Property</span></span>|<span data-ttu-id="21715-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="21715-130">Type</span></span>|<span data-ttu-id="21715-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="21715-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21715-132">accountId</span><span class="sxs-lookup"><span data-stu-id="21715-132">accountId</span></span>|<span data-ttu-id="21715-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21715-133">String</span></span>|<span data-ttu-id="21715-134">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="21715-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="21715-135">id</span><span class="sxs-lookup"><span data-stu-id="21715-135">id</span></span>|<span data-ttu-id="21715-136">String</span><span class="sxs-lookup"><span data-stu-id="21715-136">String</span></span>|<span data-ttu-id="21715-137">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="21715-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="21715-138">displayName</span><span class="sxs-lookup"><span data-stu-id="21715-138">displayName</span></span>|<span data-ttu-id="21715-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21715-139">String</span></span>|<span data-ttu-id="21715-140">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="21715-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="21715-141">description</span><span class="sxs-lookup"><span data-stu-id="21715-141">description</span></span>|<span data-ttu-id="21715-142">String</span><span class="sxs-lookup"><span data-stu-id="21715-142">String</span></span>|<span data-ttu-id="21715-143">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="21715-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="21715-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21715-144">createdDateTime</span></span>|<span data-ttu-id="21715-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21715-145">DateTimeOffset</span></span>|<span data-ttu-id="21715-146">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="21715-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="21715-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21715-147">lastModifiedDateTime</span></span>|<span data-ttu-id="21715-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21715-148">DateTimeOffset</span></span>|<span data-ttu-id="21715-149">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="21715-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="21715-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="21715-150">tokenValue</span></span>|<span data-ttu-id="21715-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21715-151">String</span></span>|<span data-ttu-id="21715-152">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="21715-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="21715-153">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="21715-153">tokenExpirationDateTime</span></span>|<span data-ttu-id="21715-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21715-154">DateTimeOffset</span></span>|<span data-ttu-id="21715-155">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="21715-155">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="21715-156">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21715-156">enrolledDeviceCount</span></span>|<span data-ttu-id="21715-157">Int32</span><span class="sxs-lookup"><span data-stu-id="21715-157">Int32</span></span>|<span data-ttu-id="21715-158">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="21715-158">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="21715-159">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="21715-159">qrCodeContent</span></span>|<span data-ttu-id="21715-160">String</span><span class="sxs-lookup"><span data-stu-id="21715-160">String</span></span>|<span data-ttu-id="21715-161">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="21715-161">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="21715-162">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="21715-162">qrCodeImage</span></span>|[<span data-ttu-id="21715-163">mimeContent</span><span class="sxs-lookup"><span data-stu-id="21715-163">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="21715-164">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="21715-164">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="21715-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="21715-165">Response</span></span>
<span data-ttu-id="21715-166">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21715-166">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21715-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21715-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="21715-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21715-168">Request</span></span>
<span data-ttu-id="21715-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21715-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="21715-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="21715-170">Response</span></span>
<span data-ttu-id="21715-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21715-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





