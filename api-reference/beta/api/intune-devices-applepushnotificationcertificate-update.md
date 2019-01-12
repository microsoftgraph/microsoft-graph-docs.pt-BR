---
title: Atualizar applePushNotificationCertificate
description: Atualizar as propriedades de um objeto applePushNotificationCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b6cc1b113b964dbc2f2ffdaae1e52639ec2463f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964834"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="8ceac-103">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="8ceac-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="8ceac-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8ceac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ceac-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8ceac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ceac-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8ceac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ceac-107">Atualizar as propriedades de um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="8ceac-107">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8ceac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8ceac-108">Prerequisites</span></span>
<span data-ttu-id="8ceac-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ceac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ceac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ceac-111">Permission type</span></span>|<span data-ttu-id="8ceac-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8ceac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ceac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ceac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ceac-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ceac-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8ceac-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ceac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ceac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ceac-116">Not supported.</span></span>|
|<span data-ttu-id="8ceac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ceac-117">Application</span></span>|<span data-ttu-id="8ceac-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ceac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ceac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ceac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="8ceac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ceac-120">Request headers</span></span>
|<span data-ttu-id="8ceac-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ceac-121">Header</span></span>|<span data-ttu-id="8ceac-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8ceac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ceac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ceac-123">Authorization</span></span>|<span data-ttu-id="8ceac-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ceac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ceac-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8ceac-125">Accept</span></span>|<span data-ttu-id="8ceac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ceac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ceac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ceac-127">Request body</span></span>
<span data-ttu-id="8ceac-128">No corpo da solicitação, forneça uma representação JSON do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="8ceac-128">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="8ceac-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="8ceac-129">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="8ceac-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ceac-130">Property</span></span>|<span data-ttu-id="8ceac-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ceac-131">Type</span></span>|<span data-ttu-id="8ceac-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ceac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ceac-133">id</span><span class="sxs-lookup"><span data-stu-id="8ceac-133">id</span></span>|<span data-ttu-id="8ceac-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ceac-134">String</span></span>|<span data-ttu-id="8ceac-135">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="8ceac-135">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="8ceac-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="8ceac-136">appleIdentifier</span></span>|<span data-ttu-id="8ceac-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ceac-137">String</span></span>|<span data-ttu-id="8ceac-138">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="8ceac-138">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="8ceac-139">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="8ceac-139">topicIdentifier</span></span>|<span data-ttu-id="8ceac-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ceac-140">String</span></span>|<span data-ttu-id="8ceac-141">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="8ceac-141">Topic Id.</span></span>|
|<span data-ttu-id="8ceac-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ceac-142">lastModifiedDateTime</span></span>|<span data-ttu-id="8ceac-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ceac-143">DateTimeOffset</span></span>|<span data-ttu-id="8ceac-144">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="8ceac-144">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="8ceac-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8ceac-145">expirationDateTime</span></span>|<span data-ttu-id="8ceac-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ceac-146">DateTimeOffset</span></span>|<span data-ttu-id="8ceac-147">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="8ceac-147">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="8ceac-148">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="8ceac-148">certificateUploadStatus</span></span>|<span data-ttu-id="8ceac-149">String</span><span class="sxs-lookup"><span data-stu-id="8ceac-149">String</span></span>|<span data-ttu-id="8ceac-150">O status de carregamento de certificado.</span><span class="sxs-lookup"><span data-stu-id="8ceac-150">The certificate upload status.</span></span>|
|<span data-ttu-id="8ceac-151">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="8ceac-151">certificateUploadFailureReason</span></span>|<span data-ttu-id="8ceac-152">String</span><span class="sxs-lookup"><span data-stu-id="8ceac-152">String</span></span>|<span data-ttu-id="8ceac-153">O motivo pelo qual o carregamento do certificado falhou.</span><span class="sxs-lookup"><span data-stu-id="8ceac-153">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="8ceac-154">certificado</span><span class="sxs-lookup"><span data-stu-id="8ceac-154">certificate</span></span>|<span data-ttu-id="8ceac-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ceac-155">String</span></span>|<span data-ttu-id="8ceac-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8ceac-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8ceac-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ceac-157">Response</span></span>
<span data-ttu-id="8ceac-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ceac-158">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ceac-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ceac-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ceac-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ceac-160">Request</span></span>
<span data-ttu-id="8ceac-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ceac-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8ceac-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ceac-162">Response</span></span>
<span data-ttu-id="8ceac-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ceac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





