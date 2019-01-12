---
title: Criar androidDeviceOwnerEnrollmentProfile
description: Crie um novo objeto de androidDeviceOwnerEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7d99ae3099baed597f58afe8ad9b44d568c2cca5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985855"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="73f84-103">Criar androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="73f84-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="73f84-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="73f84-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73f84-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="73f84-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73f84-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="73f84-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73f84-107">Crie um novo objeto de [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="73f84-107">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73f84-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73f84-108">Prerequisites</span></span>
<span data-ttu-id="73f84-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73f84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73f84-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73f84-111">Permission type</span></span>|<span data-ttu-id="73f84-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73f84-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73f84-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73f84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73f84-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73f84-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73f84-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73f84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73f84-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73f84-116">Not supported.</span></span>|
|<span data-ttu-id="73f84-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73f84-117">Application</span></span>|<span data-ttu-id="73f84-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73f84-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73f84-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73f84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="73f84-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73f84-120">Request headers</span></span>
|<span data-ttu-id="73f84-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73f84-121">Header</span></span>|<span data-ttu-id="73f84-122">Valor</span><span class="sxs-lookup"><span data-stu-id="73f84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73f84-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="73f84-123">Authorization</span></span>|<span data-ttu-id="73f84-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73f84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73f84-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73f84-125">Accept</span></span>|<span data-ttu-id="73f84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73f84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73f84-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73f84-127">Request body</span></span>
<span data-ttu-id="73f84-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidDeviceOwnerEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="73f84-128">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="73f84-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidDeviceOwnerEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="73f84-129">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="73f84-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73f84-130">Property</span></span>|<span data-ttu-id="73f84-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="73f84-131">Type</span></span>|<span data-ttu-id="73f84-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="73f84-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73f84-133">accountId</span><span class="sxs-lookup"><span data-stu-id="73f84-133">accountId</span></span>|<span data-ttu-id="73f84-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73f84-134">String</span></span>|<span data-ttu-id="73f84-135">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="73f84-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="73f84-136">id</span><span class="sxs-lookup"><span data-stu-id="73f84-136">id</span></span>|<span data-ttu-id="73f84-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73f84-137">String</span></span>|<span data-ttu-id="73f84-138">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="73f84-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="73f84-139">displayName</span><span class="sxs-lookup"><span data-stu-id="73f84-139">displayName</span></span>|<span data-ttu-id="73f84-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73f84-140">String</span></span>|<span data-ttu-id="73f84-141">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="73f84-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="73f84-142">description</span><span class="sxs-lookup"><span data-stu-id="73f84-142">description</span></span>|<span data-ttu-id="73f84-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73f84-143">String</span></span>|<span data-ttu-id="73f84-144">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="73f84-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="73f84-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73f84-145">createdDateTime</span></span>|<span data-ttu-id="73f84-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73f84-146">DateTimeOffset</span></span>|<span data-ttu-id="73f84-147">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="73f84-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="73f84-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73f84-148">lastModifiedDateTime</span></span>|<span data-ttu-id="73f84-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73f84-149">DateTimeOffset</span></span>|<span data-ttu-id="73f84-150">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="73f84-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="73f84-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="73f84-151">tokenValue</span></span>|<span data-ttu-id="73f84-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73f84-152">String</span></span>|<span data-ttu-id="73f84-153">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="73f84-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="73f84-154">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="73f84-154">tokenCreationDateTime</span></span>|<span data-ttu-id="73f84-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73f84-155">DateTimeOffset</span></span>|<span data-ttu-id="73f84-156">Data hora em que o token mais recentemente criado foi criado.</span><span class="sxs-lookup"><span data-stu-id="73f84-156">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="73f84-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="73f84-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="73f84-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73f84-158">DateTimeOffset</span></span>|<span data-ttu-id="73f84-159">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="73f84-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="73f84-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="73f84-160">enrolledDeviceCount</span></span>|<span data-ttu-id="73f84-161">Int32</span><span class="sxs-lookup"><span data-stu-id="73f84-161">Int32</span></span>|<span data-ttu-id="73f84-162">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="73f84-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="73f84-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="73f84-163">qrCodeContent</span></span>|<span data-ttu-id="73f84-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73f84-164">String</span></span>|<span data-ttu-id="73f84-165">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="73f84-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="73f84-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="73f84-166">qrCodeImage</span></span>|[<span data-ttu-id="73f84-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="73f84-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="73f84-168">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="73f84-168">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="73f84-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="73f84-169">Response</span></span>
<span data-ttu-id="73f84-170">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73f84-170">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73f84-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73f84-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="73f84-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73f84-172">Request</span></span>
<span data-ttu-id="73f84-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73f84-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
Content-type: application/json
Content-length: 629

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="73f84-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="73f84-174">Response</span></span>
<span data-ttu-id="73f84-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73f84-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





