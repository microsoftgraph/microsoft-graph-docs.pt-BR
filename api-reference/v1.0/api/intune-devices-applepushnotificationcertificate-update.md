---
title: Atualizar applePushNotificationCertificate
description: Atualizar as propriedades de um objeto applePushNotificationCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b26db969076896a8fb45dbe8d2c06894e50d0a9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009622"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="b06f2-103">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="b06f2-103">Update applePushNotificationCertificate</span></span>

<span data-ttu-id="b06f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b06f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b06f2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b06f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b06f2-106">Atualizar as propriedades de um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="b06f2-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b06f2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b06f2-107">Prerequisites</span></span>
<span data-ttu-id="b06f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b06f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b06f2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b06f2-110">Permission type</span></span>|<span data-ttu-id="b06f2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b06f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b06f2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b06f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b06f2-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b06f2-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b06f2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b06f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b06f2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b06f2-115">Not supported.</span></span>|
|<span data-ttu-id="b06f2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b06f2-116">Application</span></span>|<span data-ttu-id="b06f2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b06f2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b06f2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b06f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="b06f2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b06f2-119">Request headers</span></span>
|<span data-ttu-id="b06f2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b06f2-120">Header</span></span>|<span data-ttu-id="b06f2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b06f2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b06f2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b06f2-122">Authorization</span></span>|<span data-ttu-id="b06f2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b06f2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b06f2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b06f2-124">Accept</span></span>|<span data-ttu-id="b06f2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b06f2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b06f2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b06f2-126">Request body</span></span>
<span data-ttu-id="b06f2-127">No corpo da solicitação, forneça uma representação JSON do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="b06f2-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="b06f2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="b06f2-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="b06f2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b06f2-129">Property</span></span>|<span data-ttu-id="b06f2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b06f2-130">Type</span></span>|<span data-ttu-id="b06f2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b06f2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b06f2-132">id</span><span class="sxs-lookup"><span data-stu-id="b06f2-132">id</span></span>|<span data-ttu-id="b06f2-133">String</span><span class="sxs-lookup"><span data-stu-id="b06f2-133">String</span></span>|<span data-ttu-id="b06f2-134">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="b06f2-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="b06f2-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="b06f2-135">appleIdentifier</span></span>|<span data-ttu-id="b06f2-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b06f2-136">String</span></span>|<span data-ttu-id="b06f2-137">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="b06f2-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="b06f2-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="b06f2-138">topicIdentifier</span></span>|<span data-ttu-id="b06f2-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b06f2-139">String</span></span>|<span data-ttu-id="b06f2-140">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="b06f2-140">Topic Id.</span></span>|
|<span data-ttu-id="b06f2-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b06f2-141">lastModifiedDateTime</span></span>|<span data-ttu-id="b06f2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b06f2-142">DateTimeOffset</span></span>|<span data-ttu-id="b06f2-143">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="b06f2-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="b06f2-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b06f2-144">expirationDateTime</span></span>|<span data-ttu-id="b06f2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b06f2-145">DateTimeOffset</span></span>|<span data-ttu-id="b06f2-146">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="b06f2-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="b06f2-147">certificado</span><span class="sxs-lookup"><span data-stu-id="b06f2-147">certificate</span></span>|<span data-ttu-id="b06f2-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b06f2-148">String</span></span>|<span data-ttu-id="b06f2-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b06f2-149">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b06f2-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b06f2-150">Response</span></span>
<span data-ttu-id="b06f2-151">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b06f2-151">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b06f2-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b06f2-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="b06f2-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b06f2-153">Request</span></span>
<span data-ttu-id="b06f2-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b06f2-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="b06f2-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="b06f2-155">Response</span></span>
<span data-ttu-id="b06f2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b06f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 384

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```









