---
title: Criar androidForWorkEnrollmentProfile
description: Cria um novo objeto androidForWorkEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2890bba72a16933e0a45009a573044b65c099e9a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854197"
---
# <a name="create-androidforworkenrollmentprofile"></a><span data-ttu-id="adb7f-103">Criar androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="adb7f-103">Create androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="adb7f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="adb7f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adb7f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="adb7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="adb7f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="adb7f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="adb7f-107">Cria um novo objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="adb7f-107">Create a new [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="adb7f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="adb7f-108">Prerequisites</span></span>
<span data-ttu-id="adb7f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adb7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adb7f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="adb7f-111">Permission type</span></span>|<span data-ttu-id="adb7f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="adb7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adb7f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="adb7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="adb7f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adb7f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="adb7f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="adb7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adb7f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adb7f-116">Not supported.</span></span>|
|<span data-ttu-id="adb7f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="adb7f-117">Application</span></span>|<span data-ttu-id="adb7f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adb7f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adb7f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adb7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="adb7f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="adb7f-120">Request headers</span></span>
|<span data-ttu-id="adb7f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="adb7f-121">Header</span></span>|<span data-ttu-id="adb7f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="adb7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adb7f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="adb7f-123">Authorization</span></span>|<span data-ttu-id="adb7f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="adb7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adb7f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="adb7f-125">Accept</span></span>|<span data-ttu-id="adb7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="adb7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adb7f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="adb7f-127">Request body</span></span>
<span data-ttu-id="adb7f-128">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="adb7f-128">In the request body, supply a JSON representation for the androidForWorkEnrollmentProfile object.</span></span>

<span data-ttu-id="adb7f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="adb7f-129">The following table shows the properties that are required when you create the androidForWorkEnrollmentProfile.</span></span>

|<span data-ttu-id="adb7f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="adb7f-130">Property</span></span>|<span data-ttu-id="adb7f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="adb7f-131">Type</span></span>|<span data-ttu-id="adb7f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="adb7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adb7f-133">accountId</span><span class="sxs-lookup"><span data-stu-id="adb7f-133">accountId</span></span>|<span data-ttu-id="adb7f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="adb7f-134">String</span></span>|<span data-ttu-id="adb7f-135">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="adb7f-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="adb7f-136">id</span><span class="sxs-lookup"><span data-stu-id="adb7f-136">id</span></span>|<span data-ttu-id="adb7f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="adb7f-137">String</span></span>|<span data-ttu-id="adb7f-138">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="adb7f-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="adb7f-139">displayName</span><span class="sxs-lookup"><span data-stu-id="adb7f-139">displayName</span></span>|<span data-ttu-id="adb7f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="adb7f-140">String</span></span>|<span data-ttu-id="adb7f-141">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="adb7f-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="adb7f-142">description</span><span class="sxs-lookup"><span data-stu-id="adb7f-142">description</span></span>|<span data-ttu-id="adb7f-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="adb7f-143">String</span></span>|<span data-ttu-id="adb7f-144">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="adb7f-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="adb7f-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="adb7f-145">createdDateTime</span></span>|<span data-ttu-id="adb7f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adb7f-146">DateTimeOffset</span></span>|<span data-ttu-id="adb7f-147">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="adb7f-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="adb7f-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="adb7f-148">lastModifiedDateTime</span></span>|<span data-ttu-id="adb7f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adb7f-149">DateTimeOffset</span></span>|<span data-ttu-id="adb7f-150">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="adb7f-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="adb7f-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="adb7f-151">tokenValue</span></span>|<span data-ttu-id="adb7f-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="adb7f-152">String</span></span>|<span data-ttu-id="adb7f-153">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="adb7f-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="adb7f-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="adb7f-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="adb7f-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adb7f-155">DateTimeOffset</span></span>|<span data-ttu-id="adb7f-156">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="adb7f-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="adb7f-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="adb7f-157">enrolledDeviceCount</span></span>|<span data-ttu-id="adb7f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="adb7f-158">Int32</span></span>|<span data-ttu-id="adb7f-159">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="adb7f-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="adb7f-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="adb7f-160">qrCodeContent</span></span>|<span data-ttu-id="adb7f-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="adb7f-161">String</span></span>|<span data-ttu-id="adb7f-162">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="adb7f-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="adb7f-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="adb7f-163">qrCodeImage</span></span>|[<span data-ttu-id="adb7f-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="adb7f-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="adb7f-165">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="adb7f-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="adb7f-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="adb7f-166">Response</span></span>
<span data-ttu-id="adb7f-167">Se bem-sucedido, este método retornará um código de resposta `201 Created` e o objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="adb7f-167">If successful, this method returns a `201 Created` response code and a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adb7f-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="adb7f-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="adb7f-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="adb7f-169">Request</span></span>
<span data-ttu-id="adb7f-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="adb7f-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles
Content-type: application/json
Content-length: 560

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="adb7f-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="adb7f-171">Response</span></span>
<span data-ttu-id="adb7f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="adb7f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





