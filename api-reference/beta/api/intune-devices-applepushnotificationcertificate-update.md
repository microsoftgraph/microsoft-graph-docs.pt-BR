---
title: Atualizar applePushNotificationCertificate
description: Atualizar as propriedades de um objeto applePushNotificationCertificate.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b9eaca912e32c8575c692746040fc23535906466
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821746"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="c7085-103">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="c7085-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="c7085-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c7085-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7085-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c7085-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7085-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c7085-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7085-107">Atualizar as propriedades de um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="c7085-107">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c7085-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7085-108">Prerequisites</span></span>
<span data-ttu-id="c7085-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7085-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7085-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7085-111">Permission type</span></span>|<span data-ttu-id="c7085-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c7085-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7085-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7085-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7085-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7085-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c7085-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7085-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7085-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7085-116">Not supported.</span></span>|
|<span data-ttu-id="c7085-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7085-117">Application</span></span>|<span data-ttu-id="c7085-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7085-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7085-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7085-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="c7085-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7085-120">Request headers</span></span>
|<span data-ttu-id="c7085-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7085-121">Header</span></span>|<span data-ttu-id="c7085-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c7085-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7085-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7085-123">Authorization</span></span>|<span data-ttu-id="c7085-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7085-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7085-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7085-125">Accept</span></span>|<span data-ttu-id="c7085-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7085-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7085-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7085-127">Request body</span></span>
<span data-ttu-id="c7085-128">No corpo da solicitação, forneça uma representação JSON do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="c7085-128">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="c7085-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="c7085-129">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="c7085-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7085-130">Property</span></span>|<span data-ttu-id="c7085-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7085-131">Type</span></span>|<span data-ttu-id="c7085-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7085-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7085-133">id</span><span class="sxs-lookup"><span data-stu-id="c7085-133">id</span></span>|<span data-ttu-id="c7085-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7085-134">String</span></span>|<span data-ttu-id="c7085-135">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="c7085-135">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="c7085-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="c7085-136">appleIdentifier</span></span>|<span data-ttu-id="c7085-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7085-137">String</span></span>|<span data-ttu-id="c7085-138">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="c7085-138">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="c7085-139">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="c7085-139">topicIdentifier</span></span>|<span data-ttu-id="c7085-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7085-140">String</span></span>|<span data-ttu-id="c7085-141">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="c7085-141">Topic Id.</span></span>|
|<span data-ttu-id="c7085-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7085-142">lastModifiedDateTime</span></span>|<span data-ttu-id="c7085-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7085-143">DateTimeOffset</span></span>|<span data-ttu-id="c7085-144">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="c7085-144">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="c7085-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c7085-145">expirationDateTime</span></span>|<span data-ttu-id="c7085-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7085-146">DateTimeOffset</span></span>|<span data-ttu-id="c7085-147">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="c7085-147">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="c7085-148">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="c7085-148">certificateUploadStatus</span></span>|<span data-ttu-id="c7085-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7085-149">String</span></span>|<span data-ttu-id="c7085-150">O status de carregamento de certificado.</span><span class="sxs-lookup"><span data-stu-id="c7085-150">The certificate upload status.</span></span>|
|<span data-ttu-id="c7085-151">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="c7085-151">certificateUploadFailureReason</span></span>|<span data-ttu-id="c7085-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7085-152">String</span></span>|<span data-ttu-id="c7085-153">O motivo pelo qual o carregamento do certificado falhou.</span><span class="sxs-lookup"><span data-stu-id="c7085-153">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="c7085-154">certificado</span><span class="sxs-lookup"><span data-stu-id="c7085-154">certificate</span></span>|<span data-ttu-id="c7085-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7085-155">String</span></span>|<span data-ttu-id="c7085-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c7085-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c7085-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7085-157">Response</span></span>
<span data-ttu-id="c7085-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7085-158">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7085-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7085-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7085-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7085-160">Request</span></span>
<span data-ttu-id="c7085-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7085-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 409

{
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="c7085-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7085-162">Response</span></span>
<span data-ttu-id="c7085-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7085-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





