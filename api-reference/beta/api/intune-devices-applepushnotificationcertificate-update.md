---
title: Atualizar applePushNotificationCertificate
description: Atualizar as propriedades de um objeto applePushNotificationCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d5c82bd86b931fa619b0e92239558126df3ae0e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136493"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="9023e-103">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="9023e-103">Update applePushNotificationCertificate</span></span>

<span data-ttu-id="9023e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9023e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9023e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9023e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9023e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9023e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9023e-107">Atualizar as propriedades de um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="9023e-107">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9023e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9023e-108">Prerequisites</span></span>
<span data-ttu-id="9023e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9023e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9023e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9023e-111">Permission type</span></span>|<span data-ttu-id="9023e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9023e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9023e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9023e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9023e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9023e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9023e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9023e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9023e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9023e-116">Not supported.</span></span>|
|<span data-ttu-id="9023e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9023e-117">Application</span></span>|<span data-ttu-id="9023e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9023e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9023e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9023e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="9023e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9023e-120">Request headers</span></span>
|<span data-ttu-id="9023e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9023e-121">Header</span></span>|<span data-ttu-id="9023e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9023e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9023e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9023e-123">Authorization</span></span>|<span data-ttu-id="9023e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9023e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9023e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9023e-125">Accept</span></span>|<span data-ttu-id="9023e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9023e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9023e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9023e-127">Request body</span></span>
<span data-ttu-id="9023e-128">No corpo da solicitação, forneça uma representação JSON do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="9023e-128">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="9023e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="9023e-129">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="9023e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9023e-130">Property</span></span>|<span data-ttu-id="9023e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9023e-131">Type</span></span>|<span data-ttu-id="9023e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9023e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9023e-133">id</span><span class="sxs-lookup"><span data-stu-id="9023e-133">id</span></span>|<span data-ttu-id="9023e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9023e-134">String</span></span>|<span data-ttu-id="9023e-135">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="9023e-135">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="9023e-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="9023e-136">appleIdentifier</span></span>|<span data-ttu-id="9023e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9023e-137">String</span></span>|<span data-ttu-id="9023e-138">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="9023e-138">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="9023e-139">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="9023e-139">topicIdentifier</span></span>|<span data-ttu-id="9023e-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9023e-140">String</span></span>|<span data-ttu-id="9023e-141">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="9023e-141">Topic Id.</span></span>|
|<span data-ttu-id="9023e-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9023e-142">lastModifiedDateTime</span></span>|<span data-ttu-id="9023e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9023e-143">DateTimeOffset</span></span>|<span data-ttu-id="9023e-144">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="9023e-144">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="9023e-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9023e-145">expirationDateTime</span></span>|<span data-ttu-id="9023e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9023e-146">DateTimeOffset</span></span>|<span data-ttu-id="9023e-147">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="9023e-147">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="9023e-148">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="9023e-148">certificateUploadStatus</span></span>|<span data-ttu-id="9023e-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9023e-149">String</span></span>|<span data-ttu-id="9023e-150">O status de carregamento do certificado.</span><span class="sxs-lookup"><span data-stu-id="9023e-150">The certificate upload status.</span></span>|
|<span data-ttu-id="9023e-151">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="9023e-151">certificateUploadFailureReason</span></span>|<span data-ttu-id="9023e-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9023e-152">String</span></span>|<span data-ttu-id="9023e-153">O motivo pelo qual o carregamento do certificado falhou.</span><span class="sxs-lookup"><span data-stu-id="9023e-153">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="9023e-154">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="9023e-154">certificateSerialNumber</span></span>|<span data-ttu-id="9023e-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9023e-155">String</span></span>|<span data-ttu-id="9023e-156">Número de série do certificado.</span><span class="sxs-lookup"><span data-stu-id="9023e-156">Certificate serial number.</span></span> <span data-ttu-id="9023e-157">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9023e-157">This property is read-only.</span></span>|
|<span data-ttu-id="9023e-158">certificado</span><span class="sxs-lookup"><span data-stu-id="9023e-158">certificate</span></span>|<span data-ttu-id="9023e-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9023e-159">String</span></span>|<span data-ttu-id="9023e-160">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9023e-160">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9023e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="9023e-161">Response</span></span>
<span data-ttu-id="9023e-162">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9023e-162">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9023e-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9023e-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="9023e-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9023e-164">Request</span></span>
<span data-ttu-id="9023e-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9023e-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9023e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="9023e-166">Response</span></span>
<span data-ttu-id="9023e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9023e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




