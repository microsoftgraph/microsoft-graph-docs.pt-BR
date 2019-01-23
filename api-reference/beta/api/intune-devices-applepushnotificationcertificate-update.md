---
title: Atualizar applePushNotificationCertificate
description: Atualizar as propriedades de um objeto applePushNotificationCertificate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e14e4056f0428548e0b910c8647dc4442efe4abd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397481"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="71971-103">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="71971-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="71971-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="71971-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="71971-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="71971-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71971-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="71971-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71971-107">Atualizar as propriedades de um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="71971-107">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71971-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71971-108">Prerequisites</span></span>
<span data-ttu-id="71971-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="71971-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="71971-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71971-111">Permission type</span></span>|<span data-ttu-id="71971-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71971-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71971-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71971-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71971-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71971-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="71971-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71971-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71971-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71971-116">Not supported.</span></span>|
|<span data-ttu-id="71971-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71971-117">Application</span></span>|<span data-ttu-id="71971-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71971-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71971-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71971-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="71971-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71971-120">Request headers</span></span>
|<span data-ttu-id="71971-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71971-121">Header</span></span>|<span data-ttu-id="71971-122">Valor</span><span class="sxs-lookup"><span data-stu-id="71971-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71971-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="71971-123">Authorization</span></span>|<span data-ttu-id="71971-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71971-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71971-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71971-125">Accept</span></span>|<span data-ttu-id="71971-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71971-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71971-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71971-127">Request body</span></span>
<span data-ttu-id="71971-128">No corpo da solicitação, forneça uma representação JSON do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="71971-128">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="71971-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="71971-129">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="71971-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71971-130">Property</span></span>|<span data-ttu-id="71971-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="71971-131">Type</span></span>|<span data-ttu-id="71971-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="71971-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71971-133">id</span><span class="sxs-lookup"><span data-stu-id="71971-133">id</span></span>|<span data-ttu-id="71971-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71971-134">String</span></span>|<span data-ttu-id="71971-135">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="71971-135">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="71971-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="71971-136">appleIdentifier</span></span>|<span data-ttu-id="71971-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71971-137">String</span></span>|<span data-ttu-id="71971-138">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="71971-138">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="71971-139">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="71971-139">topicIdentifier</span></span>|<span data-ttu-id="71971-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71971-140">String</span></span>|<span data-ttu-id="71971-141">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="71971-141">Topic Id.</span></span>|
|<span data-ttu-id="71971-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71971-142">lastModifiedDateTime</span></span>|<span data-ttu-id="71971-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71971-143">DateTimeOffset</span></span>|<span data-ttu-id="71971-144">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="71971-144">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="71971-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="71971-145">expirationDateTime</span></span>|<span data-ttu-id="71971-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71971-146">DateTimeOffset</span></span>|<span data-ttu-id="71971-147">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="71971-147">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="71971-148">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="71971-148">certificateUploadStatus</span></span>|<span data-ttu-id="71971-149">String</span><span class="sxs-lookup"><span data-stu-id="71971-149">String</span></span>|<span data-ttu-id="71971-150">O status de carregamento de certificado.</span><span class="sxs-lookup"><span data-stu-id="71971-150">The certificate upload status.</span></span>|
|<span data-ttu-id="71971-151">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="71971-151">certificateUploadFailureReason</span></span>|<span data-ttu-id="71971-152">String</span><span class="sxs-lookup"><span data-stu-id="71971-152">String</span></span>|<span data-ttu-id="71971-153">O motivo pelo qual o carregamento do certificado falhou.</span><span class="sxs-lookup"><span data-stu-id="71971-153">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="71971-154">certificado</span><span class="sxs-lookup"><span data-stu-id="71971-154">certificate</span></span>|<span data-ttu-id="71971-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71971-155">String</span></span>|<span data-ttu-id="71971-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="71971-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="71971-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="71971-157">Response</span></span>
<span data-ttu-id="71971-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71971-158">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71971-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71971-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="71971-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71971-160">Request</span></span>
<span data-ttu-id="71971-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71971-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="71971-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="71971-162">Response</span></span>
<span data-ttu-id="71971-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71971-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




