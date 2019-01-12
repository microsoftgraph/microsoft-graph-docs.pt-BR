---
title: Criar androidForWorkEnrollmentProfile
description: Cria um novo objeto androidForWorkEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cc51a0a5eede602e0757571b186a7995d8f4867b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27992039"
---
# <a name="create-androidforworkenrollmentprofile"></a><span data-ttu-id="e3ee3-103">Criar androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e3ee3-103">Create androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="e3ee3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3ee3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3ee3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3ee3-107">Cria um novo objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e3ee3-107">Create a new [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3ee3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3ee3-108">Prerequisites</span></span>
<span data-ttu-id="e3ee3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3ee3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3ee3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3ee3-111">Permission type</span></span>|<span data-ttu-id="e3ee3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e3ee3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3ee3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3ee3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3ee3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3ee3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e3ee3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3ee3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3ee3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-116">Not supported.</span></span>|
|<span data-ttu-id="e3ee3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3ee3-117">Application</span></span>|<span data-ttu-id="e3ee3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3ee3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3ee3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e3ee3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3ee3-120">Request headers</span></span>
|<span data-ttu-id="e3ee3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3ee3-121">Header</span></span>|<span data-ttu-id="e3ee3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e3ee3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3ee3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3ee3-123">Authorization</span></span>|<span data-ttu-id="e3ee3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3ee3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e3ee3-125">Accept</span></span>|<span data-ttu-id="e3ee3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3ee3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3ee3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3ee3-127">Request body</span></span>
<span data-ttu-id="e3ee3-128">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-128">In the request body, supply a JSON representation for the androidForWorkEnrollmentProfile object.</span></span>

<span data-ttu-id="e3ee3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-129">The following table shows the properties that are required when you create the androidForWorkEnrollmentProfile.</span></span>

|<span data-ttu-id="e3ee3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3ee3-130">Property</span></span>|<span data-ttu-id="e3ee3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3ee3-131">Type</span></span>|<span data-ttu-id="e3ee3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3ee3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3ee3-133">accountId</span><span class="sxs-lookup"><span data-stu-id="e3ee3-133">accountId</span></span>|<span data-ttu-id="e3ee3-134">String</span><span class="sxs-lookup"><span data-stu-id="e3ee3-134">String</span></span>|<span data-ttu-id="e3ee3-135">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="e3ee3-136">id</span><span class="sxs-lookup"><span data-stu-id="e3ee3-136">id</span></span>|<span data-ttu-id="e3ee3-137">String</span><span class="sxs-lookup"><span data-stu-id="e3ee3-137">String</span></span>|<span data-ttu-id="e3ee3-138">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="e3ee3-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e3ee3-139">displayName</span></span>|<span data-ttu-id="e3ee3-140">String</span><span class="sxs-lookup"><span data-stu-id="e3ee3-140">String</span></span>|<span data-ttu-id="e3ee3-141">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="e3ee3-142">description</span><span class="sxs-lookup"><span data-stu-id="e3ee3-142">description</span></span>|<span data-ttu-id="e3ee3-143">String</span><span class="sxs-lookup"><span data-stu-id="e3ee3-143">String</span></span>|<span data-ttu-id="e3ee3-144">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="e3ee3-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3ee3-145">createdDateTime</span></span>|<span data-ttu-id="e3ee3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3ee3-146">DateTimeOffset</span></span>|<span data-ttu-id="e3ee3-147">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="e3ee3-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3ee3-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e3ee3-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3ee3-149">DateTimeOffset</span></span>|<span data-ttu-id="e3ee3-150">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="e3ee3-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="e3ee3-151">tokenValue</span></span>|<span data-ttu-id="e3ee3-152">String</span><span class="sxs-lookup"><span data-stu-id="e3ee3-152">String</span></span>|<span data-ttu-id="e3ee3-153">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="e3ee3-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e3ee3-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="e3ee3-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3ee3-155">DateTimeOffset</span></span>|<span data-ttu-id="e3ee3-156">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="e3ee3-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3ee3-157">enrolledDeviceCount</span></span>|<span data-ttu-id="e3ee3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e3ee3-158">Int32</span></span>|<span data-ttu-id="e3ee3-159">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="e3ee3-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="e3ee3-160">qrCodeContent</span></span>|<span data-ttu-id="e3ee3-161">String</span><span class="sxs-lookup"><span data-stu-id="e3ee3-161">String</span></span>|<span data-ttu-id="e3ee3-162">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="e3ee3-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="e3ee3-163">qrCodeImage</span></span>|[<span data-ttu-id="e3ee3-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e3ee3-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e3ee3-165">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="e3ee3-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3ee3-166">Response</span></span>
<span data-ttu-id="e3ee3-167">Se bem-sucedido, este método retornará um código de resposta `201 Created` e o objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-167">If successful, this method returns a `201 Created` response code and a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3ee3-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3ee3-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3ee3-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3ee3-169">Request</span></span>
<span data-ttu-id="e3ee3-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e3ee3-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3ee3-171">Response</span></span>
<span data-ttu-id="e3ee3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3ee3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





