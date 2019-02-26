---
title: Atualizar applePushNotificationCertificate
description: Atualizar as propriedades de um objeto applePushNotificationCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee760b38c8f684c0ca7f0c8bcca0c98d8a87d931
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172041"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="5cd9e-103">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="5cd9e-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="5cd9e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5cd9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cd9e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5cd9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cd9e-106">Atualizar as propriedades de um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="5cd9e-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cd9e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5cd9e-107">Prerequisites</span></span>
<span data-ttu-id="5cd9e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5cd9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5cd9e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5cd9e-110">Permission type</span></span>|<span data-ttu-id="5cd9e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5cd9e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cd9e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5cd9e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5cd9e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cd9e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5cd9e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5cd9e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cd9e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5cd9e-115">Not supported.</span></span>|
|<span data-ttu-id="5cd9e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5cd9e-116">Application</span></span>|<span data-ttu-id="5cd9e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5cd9e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cd9e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5cd9e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="5cd9e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5cd9e-119">Request headers</span></span>
|<span data-ttu-id="5cd9e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5cd9e-120">Header</span></span>|<span data-ttu-id="5cd9e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5cd9e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cd9e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5cd9e-122">Authorization</span></span>|<span data-ttu-id="5cd9e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5cd9e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cd9e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5cd9e-124">Accept</span></span>|<span data-ttu-id="5cd9e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5cd9e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cd9e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5cd9e-126">Request body</span></span>
<span data-ttu-id="5cd9e-127">No corpo da solicitação, forneça uma representação JSON do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="5cd9e-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="5cd9e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="5cd9e-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="5cd9e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5cd9e-129">Property</span></span>|<span data-ttu-id="5cd9e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cd9e-130">Type</span></span>|<span data-ttu-id="5cd9e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cd9e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cd9e-132">id</span><span class="sxs-lookup"><span data-stu-id="5cd9e-132">id</span></span>|<span data-ttu-id="5cd9e-133">String</span><span class="sxs-lookup"><span data-stu-id="5cd9e-133">String</span></span>|<span data-ttu-id="5cd9e-134">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="5cd9e-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="5cd9e-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="5cd9e-135">appleIdentifier</span></span>|<span data-ttu-id="5cd9e-136">String</span><span class="sxs-lookup"><span data-stu-id="5cd9e-136">String</span></span>|<span data-ttu-id="5cd9e-137">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="5cd9e-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="5cd9e-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="5cd9e-138">topicIdentifier</span></span>|<span data-ttu-id="5cd9e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5cd9e-139">String</span></span>|<span data-ttu-id="5cd9e-140">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="5cd9e-140">Topic Id.</span></span>|
|<span data-ttu-id="5cd9e-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cd9e-141">lastModifiedDateTime</span></span>|<span data-ttu-id="5cd9e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cd9e-142">DateTimeOffset</span></span>|<span data-ttu-id="5cd9e-143">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="5cd9e-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="5cd9e-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5cd9e-144">expirationDateTime</span></span>|<span data-ttu-id="5cd9e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cd9e-145">DateTimeOffset</span></span>|<span data-ttu-id="5cd9e-146">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="5cd9e-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="5cd9e-147">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="5cd9e-147">certificateUploadStatus</span></span>|<span data-ttu-id="5cd9e-148">String</span><span class="sxs-lookup"><span data-stu-id="5cd9e-148">String</span></span>|<span data-ttu-id="5cd9e-149">O status do carregamento do certificado.</span><span class="sxs-lookup"><span data-stu-id="5cd9e-149">The certificate upload status.</span></span>|
|<span data-ttu-id="5cd9e-150">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="5cd9e-150">certificateUploadFailureReason</span></span>|<span data-ttu-id="5cd9e-151">String</span><span class="sxs-lookup"><span data-stu-id="5cd9e-151">String</span></span>|<span data-ttu-id="5cd9e-152">O motivo da falha no carregamento do certificado.</span><span class="sxs-lookup"><span data-stu-id="5cd9e-152">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="5cd9e-153">certificado</span><span class="sxs-lookup"><span data-stu-id="5cd9e-153">certificate</span></span>|<span data-ttu-id="5cd9e-154">String</span><span class="sxs-lookup"><span data-stu-id="5cd9e-154">String</span></span>|<span data-ttu-id="5cd9e-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5cd9e-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5cd9e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cd9e-156">Response</span></span>
<span data-ttu-id="5cd9e-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5cd9e-157">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cd9e-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5cd9e-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cd9e-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5cd9e-159">Request</span></span>
<span data-ttu-id="5cd9e-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5cd9e-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 416

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="5cd9e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cd9e-161">Response</span></span>
<span data-ttu-id="5cd9e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5cd9e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificate": "Certificate value"
}
```




