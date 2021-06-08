---
title: Atualizar applePushNotificationCertificate
description: Atualizar as propriedades de um objeto applePushNotificationCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fe39b333f9768837c9ddafd808d33aa67af6ecb2
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760395"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="7576a-103">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="7576a-103">Update applePushNotificationCertificate</span></span>

<span data-ttu-id="7576a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7576a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7576a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7576a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7576a-106">Atualizar as propriedades de um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="7576a-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7576a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7576a-107">Prerequisites</span></span>
<span data-ttu-id="7576a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7576a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7576a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7576a-110">Permission type</span></span>|<span data-ttu-id="7576a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7576a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7576a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7576a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7576a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7576a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7576a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7576a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7576a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7576a-115">Not supported.</span></span>|
|<span data-ttu-id="7576a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7576a-116">Application</span></span>|<span data-ttu-id="7576a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7576a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7576a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7576a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="7576a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7576a-119">Request headers</span></span>
|<span data-ttu-id="7576a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7576a-120">Header</span></span>|<span data-ttu-id="7576a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7576a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7576a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7576a-122">Authorization</span></span>|<span data-ttu-id="7576a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7576a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7576a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7576a-124">Accept</span></span>|<span data-ttu-id="7576a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7576a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7576a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7576a-126">Request body</span></span>
<span data-ttu-id="7576a-127">No corpo da solicitação, forneça uma representação JSON do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="7576a-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="7576a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="7576a-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="7576a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7576a-129">Property</span></span>|<span data-ttu-id="7576a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7576a-130">Type</span></span>|<span data-ttu-id="7576a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7576a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7576a-132">id</span><span class="sxs-lookup"><span data-stu-id="7576a-132">id</span></span>|<span data-ttu-id="7576a-133">String</span><span class="sxs-lookup"><span data-stu-id="7576a-133">String</span></span>|<span data-ttu-id="7576a-134">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="7576a-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="7576a-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="7576a-135">appleIdentifier</span></span>|<span data-ttu-id="7576a-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7576a-136">String</span></span>|<span data-ttu-id="7576a-137">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="7576a-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="7576a-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="7576a-138">topicIdentifier</span></span>|<span data-ttu-id="7576a-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7576a-139">String</span></span>|<span data-ttu-id="7576a-140">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="7576a-140">Topic Id.</span></span>|
|<span data-ttu-id="7576a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7576a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="7576a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7576a-142">DateTimeOffset</span></span>|<span data-ttu-id="7576a-143">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="7576a-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="7576a-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7576a-144">expirationDateTime</span></span>|<span data-ttu-id="7576a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7576a-145">DateTimeOffset</span></span>|<span data-ttu-id="7576a-146">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="7576a-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="7576a-147">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="7576a-147">certificateSerialNumber</span></span>|<span data-ttu-id="7576a-148">String</span><span class="sxs-lookup"><span data-stu-id="7576a-148">String</span></span>|<span data-ttu-id="7576a-149">Número de série do certificado.</span><span class="sxs-lookup"><span data-stu-id="7576a-149">Certificate serial number.</span></span> <span data-ttu-id="7576a-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7576a-150">This property is read-only.</span></span>|
|<span data-ttu-id="7576a-151">certificado</span><span class="sxs-lookup"><span data-stu-id="7576a-151">certificate</span></span>|<span data-ttu-id="7576a-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7576a-152">String</span></span>|<span data-ttu-id="7576a-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7576a-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7576a-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="7576a-154">Response</span></span>
<span data-ttu-id="7576a-155">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7576a-155">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7576a-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7576a-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="7576a-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7576a-157">Request</span></span>
<span data-ttu-id="7576a-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7576a-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 336

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="7576a-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="7576a-159">Response</span></span>
<span data-ttu-id="7576a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7576a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 449

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificate": "Certificate value"
}
```




