---
title: Atualizar androidForWorkEnrollmentProfile
description: Atualizar as propriedades de um objeto androidForWorkEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 98d017ca961a012c195e1e729bf4a2527e50f5e0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398013"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="2f384-103">Atualizar androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="2f384-103">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="2f384-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2f384-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2f384-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2f384-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f384-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2f384-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f384-107">Atualizar as propriedades de um objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="2f384-107">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f384-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f384-108">Prerequisites</span></span>
<span data-ttu-id="2f384-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f384-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2f384-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f384-111">Permission type</span></span>|<span data-ttu-id="2f384-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f384-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f384-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f384-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f384-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f384-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f384-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f384-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f384-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f384-116">Not supported.</span></span>|
|<span data-ttu-id="2f384-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f384-117">Application</span></span>|<span data-ttu-id="2f384-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f384-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f384-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f384-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="2f384-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f384-120">Request headers</span></span>
|<span data-ttu-id="2f384-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f384-121">Header</span></span>|<span data-ttu-id="2f384-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2f384-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f384-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f384-123">Authorization</span></span>|<span data-ttu-id="2f384-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f384-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f384-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f384-125">Accept</span></span>|<span data-ttu-id="2f384-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f384-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f384-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f384-127">Request body</span></span>
<span data-ttu-id="2f384-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="2f384-128">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="2f384-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="2f384-129">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="2f384-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f384-130">Property</span></span>|<span data-ttu-id="2f384-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f384-131">Type</span></span>|<span data-ttu-id="2f384-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f384-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f384-133">accountId</span><span class="sxs-lookup"><span data-stu-id="2f384-133">accountId</span></span>|<span data-ttu-id="2f384-134">String</span><span class="sxs-lookup"><span data-stu-id="2f384-134">String</span></span>|<span data-ttu-id="2f384-135">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="2f384-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="2f384-136">id</span><span class="sxs-lookup"><span data-stu-id="2f384-136">id</span></span>|<span data-ttu-id="2f384-137">String</span><span class="sxs-lookup"><span data-stu-id="2f384-137">String</span></span>|<span data-ttu-id="2f384-138">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="2f384-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="2f384-139">displayName</span><span class="sxs-lookup"><span data-stu-id="2f384-139">displayName</span></span>|<span data-ttu-id="2f384-140">String</span><span class="sxs-lookup"><span data-stu-id="2f384-140">String</span></span>|<span data-ttu-id="2f384-141">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="2f384-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="2f384-142">description</span><span class="sxs-lookup"><span data-stu-id="2f384-142">description</span></span>|<span data-ttu-id="2f384-143">String</span><span class="sxs-lookup"><span data-stu-id="2f384-143">String</span></span>|<span data-ttu-id="2f384-144">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="2f384-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="2f384-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f384-145">createdDateTime</span></span>|<span data-ttu-id="2f384-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f384-146">DateTimeOffset</span></span>|<span data-ttu-id="2f384-147">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="2f384-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="2f384-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f384-148">lastModifiedDateTime</span></span>|<span data-ttu-id="2f384-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f384-149">DateTimeOffset</span></span>|<span data-ttu-id="2f384-150">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="2f384-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="2f384-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="2f384-151">tokenValue</span></span>|<span data-ttu-id="2f384-152">String</span><span class="sxs-lookup"><span data-stu-id="2f384-152">String</span></span>|<span data-ttu-id="2f384-153">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="2f384-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="2f384-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2f384-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="2f384-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f384-155">DateTimeOffset</span></span>|<span data-ttu-id="2f384-156">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="2f384-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="2f384-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2f384-157">enrolledDeviceCount</span></span>|<span data-ttu-id="2f384-158">Int32</span><span class="sxs-lookup"><span data-stu-id="2f384-158">Int32</span></span>|<span data-ttu-id="2f384-159">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="2f384-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="2f384-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="2f384-160">qrCodeContent</span></span>|<span data-ttu-id="2f384-161">String</span><span class="sxs-lookup"><span data-stu-id="2f384-161">String</span></span>|<span data-ttu-id="2f384-162">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="2f384-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="2f384-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="2f384-163">qrCodeImage</span></span>|[<span data-ttu-id="2f384-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2f384-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2f384-165">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="2f384-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="2f384-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f384-166">Response</span></span>
<span data-ttu-id="2f384-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f384-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f384-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f384-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f384-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f384-169">Request</span></span>
<span data-ttu-id="2f384-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f384-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f384-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f384-171">Response</span></span>
<span data-ttu-id="2f384-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f384-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




