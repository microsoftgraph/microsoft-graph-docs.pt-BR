---
title: Atualizar applePushNotificationCertificate
description: Atualizar as propriedades de um objeto applePushNotificationCertificate.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 25f6a89f028604ee5a3ca13394c6050c9553f3c8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814782"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="e8ec4-103">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="e8ec4-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="e8ec4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8ec4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8ec4-106">Atualizar as propriedades de um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="e8ec4-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8ec4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8ec4-107">Prerequisites</span></span>
<span data-ttu-id="e8ec4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8ec4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8ec4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8ec4-110">Permission type</span></span>|<span data-ttu-id="e8ec4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8ec4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8ec4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8ec4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8ec4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8ec4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e8ec4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8ec4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8ec4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-115">Not supported.</span></span>|
|<span data-ttu-id="e8ec4-116">Application</span><span class="sxs-lookup"><span data-stu-id="e8ec4-116">Application</span></span>|<span data-ttu-id="e8ec4-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8ec4-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8ec4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8ec4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="e8ec4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8ec4-119">Request headers</span></span>
|<span data-ttu-id="e8ec4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8ec4-120">Header</span></span>|<span data-ttu-id="e8ec4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e8ec4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8ec4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8ec4-122">Authorization</span></span>|<span data-ttu-id="e8ec4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8ec4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8ec4-124">Accept</span></span>|<span data-ttu-id="e8ec4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8ec4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8ec4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8ec4-126">Request body</span></span>
<span data-ttu-id="e8ec4-127">No corpo da solicitação, forneça uma representação JSON do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="e8ec4-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="e8ec4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="e8ec4-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="e8ec4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8ec4-129">Property</span></span>|<span data-ttu-id="e8ec4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8ec4-130">Type</span></span>|<span data-ttu-id="e8ec4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8ec4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8ec4-132">id</span><span class="sxs-lookup"><span data-stu-id="e8ec4-132">id</span></span>|<span data-ttu-id="e8ec4-133">String</span><span class="sxs-lookup"><span data-stu-id="e8ec4-133">String</span></span>|<span data-ttu-id="e8ec4-134">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="e8ec4-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="e8ec4-135">appleIdentifier</span></span>|<span data-ttu-id="e8ec4-136">String</span><span class="sxs-lookup"><span data-stu-id="e8ec4-136">String</span></span>|<span data-ttu-id="e8ec4-137">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="e8ec4-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="e8ec4-138">topicIdentifier</span></span>|<span data-ttu-id="e8ec4-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8ec4-139">String</span></span>|<span data-ttu-id="e8ec4-140">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-140">Topic Id.</span></span>|
|<span data-ttu-id="e8ec4-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8ec4-141">lastModifiedDateTime</span></span>|<span data-ttu-id="e8ec4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8ec4-142">DateTimeOffset</span></span>|<span data-ttu-id="e8ec4-143">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="e8ec4-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e8ec4-144">expirationDateTime</span></span>|<span data-ttu-id="e8ec4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8ec4-145">DateTimeOffset</span></span>|<span data-ttu-id="e8ec4-146">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="e8ec4-147">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="e8ec4-147">certificateUploadStatus</span></span>|<span data-ttu-id="e8ec4-148">String</span><span class="sxs-lookup"><span data-stu-id="e8ec4-148">String</span></span>|<span data-ttu-id="e8ec4-149">O status do carregamento do certificado.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-149">The certificate upload status.</span></span>|
|<span data-ttu-id="e8ec4-150">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="e8ec4-150">certificateUploadFailureReason</span></span>|<span data-ttu-id="e8ec4-151">String</span><span class="sxs-lookup"><span data-stu-id="e8ec4-151">String</span></span>|<span data-ttu-id="e8ec4-152">O motivo da falha no carregamento do certificado.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-152">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="e8ec4-153">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="e8ec4-153">certificateSerialNumber</span></span>|<span data-ttu-id="e8ec4-154">String</span><span class="sxs-lookup"><span data-stu-id="e8ec4-154">String</span></span>|<span data-ttu-id="e8ec4-155">Número de série do certificado.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-155">Certificate serial number.</span></span> <span data-ttu-id="e8ec4-156">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-156">This property is read-only.</span></span>|
|<span data-ttu-id="e8ec4-157">certificado</span><span class="sxs-lookup"><span data-stu-id="e8ec4-157">certificate</span></span>|<span data-ttu-id="e8ec4-158">String</span><span class="sxs-lookup"><span data-stu-id="e8ec4-158">String</span></span>|<span data-ttu-id="e8ec4-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e8ec4-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e8ec4-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8ec4-160">Response</span></span>
<span data-ttu-id="e8ec4-161">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-161">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8ec4-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8ec4-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8ec4-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8ec4-163">Request</span></span>
<span data-ttu-id="e8ec4-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 481

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="e8ec4-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8ec4-165">Response</span></span>
<span data-ttu-id="e8ec4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8ec4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 594

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificate": "Certificate value"
}
```




