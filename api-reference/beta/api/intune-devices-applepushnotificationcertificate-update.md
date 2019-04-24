---
title: Atualizar applePushNotificationCertificate
description: Atualizar as propriedades de um objeto applePushNotificationCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d87a60747fce6eb85cb50439eb14f14a207280d8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466137"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="b4ff3-103">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="b4ff3-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="b4ff3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b4ff3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4ff3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4ff3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4ff3-106">Atualizar as propriedades de um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="b4ff3-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4ff3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4ff3-107">Prerequisites</span></span>
<span data-ttu-id="b4ff3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4ff3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4ff3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4ff3-110">Permission type</span></span>|<span data-ttu-id="b4ff3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4ff3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4ff3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4ff3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b4ff3-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4ff3-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b4ff3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4ff3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4ff3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4ff3-115">Not supported.</span></span>|
|<span data-ttu-id="b4ff3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4ff3-116">Application</span></span>|<span data-ttu-id="b4ff3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4ff3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4ff3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4ff3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="b4ff3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4ff3-119">Request headers</span></span>
|<span data-ttu-id="b4ff3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4ff3-120">Header</span></span>|<span data-ttu-id="b4ff3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b4ff3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4ff3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4ff3-122">Authorization</span></span>|<span data-ttu-id="b4ff3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4ff3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4ff3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b4ff3-124">Accept</span></span>|<span data-ttu-id="b4ff3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b4ff3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4ff3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4ff3-126">Request body</span></span>
<span data-ttu-id="b4ff3-127">No corpo da solicitação, forneça uma representação JSON do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="b4ff3-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="b4ff3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="b4ff3-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="b4ff3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4ff3-129">Property</span></span>|<span data-ttu-id="b4ff3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4ff3-130">Type</span></span>|<span data-ttu-id="b4ff3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4ff3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4ff3-132">id</span><span class="sxs-lookup"><span data-stu-id="b4ff3-132">id</span></span>|<span data-ttu-id="b4ff3-133">String</span><span class="sxs-lookup"><span data-stu-id="b4ff3-133">String</span></span>|<span data-ttu-id="b4ff3-134">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="b4ff3-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="b4ff3-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="b4ff3-135">appleIdentifier</span></span>|<span data-ttu-id="b4ff3-136">String</span><span class="sxs-lookup"><span data-stu-id="b4ff3-136">String</span></span>|<span data-ttu-id="b4ff3-137">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="b4ff3-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="b4ff3-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="b4ff3-138">topicIdentifier</span></span>|<span data-ttu-id="b4ff3-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4ff3-139">String</span></span>|<span data-ttu-id="b4ff3-140">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="b4ff3-140">Topic Id.</span></span>|
|<span data-ttu-id="b4ff3-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4ff3-141">lastModifiedDateTime</span></span>|<span data-ttu-id="b4ff3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4ff3-142">DateTimeOffset</span></span>|<span data-ttu-id="b4ff3-143">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="b4ff3-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="b4ff3-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b4ff3-144">expirationDateTime</span></span>|<span data-ttu-id="b4ff3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4ff3-145">DateTimeOffset</span></span>|<span data-ttu-id="b4ff3-146">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="b4ff3-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="b4ff3-147">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="b4ff3-147">certificateUploadStatus</span></span>|<span data-ttu-id="b4ff3-148">String</span><span class="sxs-lookup"><span data-stu-id="b4ff3-148">String</span></span>|<span data-ttu-id="b4ff3-149">O status do carregamento do certificado.</span><span class="sxs-lookup"><span data-stu-id="b4ff3-149">The certificate upload status.</span></span>|
|<span data-ttu-id="b4ff3-150">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="b4ff3-150">certificateUploadFailureReason</span></span>|<span data-ttu-id="b4ff3-151">String</span><span class="sxs-lookup"><span data-stu-id="b4ff3-151">String</span></span>|<span data-ttu-id="b4ff3-152">O motivo da falha no carregamento do certificado.</span><span class="sxs-lookup"><span data-stu-id="b4ff3-152">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="b4ff3-153">certificado</span><span class="sxs-lookup"><span data-stu-id="b4ff3-153">certificate</span></span>|<span data-ttu-id="b4ff3-154">String</span><span class="sxs-lookup"><span data-stu-id="b4ff3-154">String</span></span>|<span data-ttu-id="b4ff3-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b4ff3-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b4ff3-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4ff3-156">Response</span></span>
<span data-ttu-id="b4ff3-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4ff3-157">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4ff3-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4ff3-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4ff3-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4ff3-159">Request</span></span>
<span data-ttu-id="b4ff3-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4ff3-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b4ff3-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4ff3-161">Response</span></span>
<span data-ttu-id="b4ff3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4ff3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





