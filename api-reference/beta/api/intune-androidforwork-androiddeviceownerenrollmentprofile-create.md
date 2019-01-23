---
title: Criar androidDeviceOwnerEnrollmentProfile
description: Crie um novo objeto de androidDeviceOwnerEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a0c766106d4467e54bda3465ff360bfcadfe71c6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401989"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="07947-103">Criar androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="07947-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="07947-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="07947-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="07947-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="07947-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07947-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="07947-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07947-107">Crie um novo objeto de [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="07947-107">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07947-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07947-108">Prerequisites</span></span>
<span data-ttu-id="07947-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="07947-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="07947-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07947-111">Permission type</span></span>|<span data-ttu-id="07947-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07947-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07947-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07947-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07947-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07947-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="07947-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07947-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07947-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07947-116">Not supported.</span></span>|
|<span data-ttu-id="07947-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07947-117">Application</span></span>|<span data-ttu-id="07947-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07947-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07947-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07947-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="07947-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07947-120">Request headers</span></span>
|<span data-ttu-id="07947-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07947-121">Header</span></span>|<span data-ttu-id="07947-122">Valor</span><span class="sxs-lookup"><span data-stu-id="07947-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07947-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="07947-123">Authorization</span></span>|<span data-ttu-id="07947-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07947-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07947-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07947-125">Accept</span></span>|<span data-ttu-id="07947-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07947-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07947-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07947-127">Request body</span></span>
<span data-ttu-id="07947-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidDeviceOwnerEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="07947-128">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="07947-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidDeviceOwnerEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="07947-129">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="07947-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07947-130">Property</span></span>|<span data-ttu-id="07947-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="07947-131">Type</span></span>|<span data-ttu-id="07947-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="07947-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07947-133">accountId</span><span class="sxs-lookup"><span data-stu-id="07947-133">accountId</span></span>|<span data-ttu-id="07947-134">String</span><span class="sxs-lookup"><span data-stu-id="07947-134">String</span></span>|<span data-ttu-id="07947-135">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="07947-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="07947-136">id</span><span class="sxs-lookup"><span data-stu-id="07947-136">id</span></span>|<span data-ttu-id="07947-137">String</span><span class="sxs-lookup"><span data-stu-id="07947-137">String</span></span>|<span data-ttu-id="07947-138">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="07947-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="07947-139">displayName</span><span class="sxs-lookup"><span data-stu-id="07947-139">displayName</span></span>|<span data-ttu-id="07947-140">String</span><span class="sxs-lookup"><span data-stu-id="07947-140">String</span></span>|<span data-ttu-id="07947-141">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="07947-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="07947-142">description</span><span class="sxs-lookup"><span data-stu-id="07947-142">description</span></span>|<span data-ttu-id="07947-143">String</span><span class="sxs-lookup"><span data-stu-id="07947-143">String</span></span>|<span data-ttu-id="07947-144">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="07947-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="07947-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07947-145">createdDateTime</span></span>|<span data-ttu-id="07947-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07947-146">DateTimeOffset</span></span>|<span data-ttu-id="07947-147">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="07947-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="07947-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07947-148">lastModifiedDateTime</span></span>|<span data-ttu-id="07947-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07947-149">DateTimeOffset</span></span>|<span data-ttu-id="07947-150">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="07947-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="07947-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="07947-151">tokenValue</span></span>|<span data-ttu-id="07947-152">String</span><span class="sxs-lookup"><span data-stu-id="07947-152">String</span></span>|<span data-ttu-id="07947-153">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="07947-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="07947-154">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="07947-154">tokenCreationDateTime</span></span>|<span data-ttu-id="07947-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07947-155">DateTimeOffset</span></span>|<span data-ttu-id="07947-156">Data hora em que o token mais recentemente criado foi criado.</span><span class="sxs-lookup"><span data-stu-id="07947-156">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="07947-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="07947-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="07947-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07947-158">DateTimeOffset</span></span>|<span data-ttu-id="07947-159">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="07947-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="07947-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07947-160">enrolledDeviceCount</span></span>|<span data-ttu-id="07947-161">Int32</span><span class="sxs-lookup"><span data-stu-id="07947-161">Int32</span></span>|<span data-ttu-id="07947-162">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="07947-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="07947-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="07947-163">qrCodeContent</span></span>|<span data-ttu-id="07947-164">String</span><span class="sxs-lookup"><span data-stu-id="07947-164">String</span></span>|<span data-ttu-id="07947-165">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="07947-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="07947-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="07947-166">qrCodeImage</span></span>|[<span data-ttu-id="07947-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="07947-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="07947-168">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="07947-168">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="07947-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="07947-169">Response</span></span>
<span data-ttu-id="07947-170">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07947-170">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07947-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07947-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="07947-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07947-172">Request</span></span>
<span data-ttu-id="07947-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07947-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="07947-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="07947-174">Response</span></span>
<span data-ttu-id="07947-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07947-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




