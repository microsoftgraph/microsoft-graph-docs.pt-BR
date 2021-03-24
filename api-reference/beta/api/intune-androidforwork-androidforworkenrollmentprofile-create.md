---
title: Criar androidForWorkEnrollmentProfile
description: Cria um novo objeto androidForWorkEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 968ef612532e568e7d34e6bbc293ea90538690a2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144729"
---
# <a name="create-androidforworkenrollmentprofile"></a><span data-ttu-id="59ff1-103">Criar androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="59ff1-103">Create androidForWorkEnrollmentProfile</span></span>

<span data-ttu-id="59ff1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59ff1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59ff1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59ff1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59ff1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59ff1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59ff1-107">Cria um novo objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="59ff1-107">Create a new [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59ff1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59ff1-108">Prerequisites</span></span>
<span data-ttu-id="59ff1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59ff1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59ff1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59ff1-111">Permission type</span></span>|<span data-ttu-id="59ff1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59ff1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59ff1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59ff1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59ff1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59ff1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="59ff1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59ff1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59ff1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59ff1-116">Not supported.</span></span>|
|<span data-ttu-id="59ff1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59ff1-117">Application</span></span>|<span data-ttu-id="59ff1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59ff1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59ff1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59ff1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="59ff1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59ff1-120">Request headers</span></span>
|<span data-ttu-id="59ff1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59ff1-121">Header</span></span>|<span data-ttu-id="59ff1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="59ff1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59ff1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="59ff1-123">Authorization</span></span>|<span data-ttu-id="59ff1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59ff1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59ff1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="59ff1-125">Accept</span></span>|<span data-ttu-id="59ff1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="59ff1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59ff1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59ff1-127">Request body</span></span>
<span data-ttu-id="59ff1-128">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="59ff1-128">In the request body, supply a JSON representation for the androidForWorkEnrollmentProfile object.</span></span>

<span data-ttu-id="59ff1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="59ff1-129">The following table shows the properties that are required when you create the androidForWorkEnrollmentProfile.</span></span>

|<span data-ttu-id="59ff1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59ff1-130">Property</span></span>|<span data-ttu-id="59ff1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="59ff1-131">Type</span></span>|<span data-ttu-id="59ff1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="59ff1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59ff1-133">accountId</span><span class="sxs-lookup"><span data-stu-id="59ff1-133">accountId</span></span>|<span data-ttu-id="59ff1-134">String</span><span class="sxs-lookup"><span data-stu-id="59ff1-134">String</span></span>|<span data-ttu-id="59ff1-135">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="59ff1-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="59ff1-136">id</span><span class="sxs-lookup"><span data-stu-id="59ff1-136">id</span></span>|<span data-ttu-id="59ff1-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59ff1-137">String</span></span>|<span data-ttu-id="59ff1-138">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="59ff1-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="59ff1-139">displayName</span><span class="sxs-lookup"><span data-stu-id="59ff1-139">displayName</span></span>|<span data-ttu-id="59ff1-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59ff1-140">String</span></span>|<span data-ttu-id="59ff1-141">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="59ff1-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="59ff1-142">descrição</span><span class="sxs-lookup"><span data-stu-id="59ff1-142">description</span></span>|<span data-ttu-id="59ff1-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59ff1-143">String</span></span>|<span data-ttu-id="59ff1-144">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="59ff1-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="59ff1-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59ff1-145">createdDateTime</span></span>|<span data-ttu-id="59ff1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59ff1-146">DateTimeOffset</span></span>|<span data-ttu-id="59ff1-147">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="59ff1-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="59ff1-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59ff1-148">lastModifiedDateTime</span></span>|<span data-ttu-id="59ff1-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59ff1-149">DateTimeOffset</span></span>|<span data-ttu-id="59ff1-150">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="59ff1-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="59ff1-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="59ff1-151">tokenValue</span></span>|<span data-ttu-id="59ff1-152">String</span><span class="sxs-lookup"><span data-stu-id="59ff1-152">String</span></span>|<span data-ttu-id="59ff1-153">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="59ff1-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="59ff1-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="59ff1-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="59ff1-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59ff1-155">DateTimeOffset</span></span>|<span data-ttu-id="59ff1-156">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="59ff1-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="59ff1-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59ff1-157">enrolledDeviceCount</span></span>|<span data-ttu-id="59ff1-158">Int32</span><span class="sxs-lookup"><span data-stu-id="59ff1-158">Int32</span></span>|<span data-ttu-id="59ff1-159">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="59ff1-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="59ff1-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="59ff1-160">qrCodeContent</span></span>|<span data-ttu-id="59ff1-161">String</span><span class="sxs-lookup"><span data-stu-id="59ff1-161">String</span></span>|<span data-ttu-id="59ff1-162">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="59ff1-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="59ff1-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="59ff1-163">qrCodeImage</span></span>|[<span data-ttu-id="59ff1-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="59ff1-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="59ff1-165">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="59ff1-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="59ff1-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="59ff1-166">Response</span></span>
<span data-ttu-id="59ff1-167">Se bem-sucedido, este método retornará um código de resposta `201 Created` e o objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59ff1-167">If successful, this method returns a `201 Created` response code and a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59ff1-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59ff1-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="59ff1-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59ff1-169">Request</span></span>
<span data-ttu-id="59ff1-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59ff1-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="59ff1-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="59ff1-171">Response</span></span>
<span data-ttu-id="59ff1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59ff1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




