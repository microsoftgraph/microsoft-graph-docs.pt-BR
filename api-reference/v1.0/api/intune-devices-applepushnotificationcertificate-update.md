---
title: Atualizar applePushNotificationCertificate
description: Atualizar as propriedades de um objeto applePushNotificationCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 128769688dcde3f6549ee2d0963853892fd7efa2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986625"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="1a705-103">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="1a705-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="1a705-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1a705-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a705-105">Atualizar as propriedades de um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="1a705-105">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a705-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1a705-106">Prerequisites</span></span>
<span data-ttu-id="1a705-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a705-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a705-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a705-109">Permission type</span></span>|<span data-ttu-id="1a705-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1a705-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a705-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a705-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1a705-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a705-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1a705-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a705-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a705-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a705-114">Not supported.</span></span>|
|<span data-ttu-id="1a705-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a705-115">Application</span></span>|<span data-ttu-id="1a705-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a705-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a705-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a705-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="1a705-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a705-118">Request headers</span></span>
|<span data-ttu-id="1a705-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1a705-119">Header</span></span>|<span data-ttu-id="1a705-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1a705-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a705-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a705-121">Authorization</span></span>|<span data-ttu-id="1a705-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a705-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a705-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1a705-123">Accept</span></span>|<span data-ttu-id="1a705-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1a705-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a705-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a705-125">Request body</span></span>
<span data-ttu-id="1a705-126">No corpo da solicitação, forneça uma representação JSON do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="1a705-126">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="1a705-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="1a705-127">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="1a705-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a705-128">Property</span></span>|<span data-ttu-id="1a705-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a705-129">Type</span></span>|<span data-ttu-id="1a705-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a705-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a705-131">id</span><span class="sxs-lookup"><span data-stu-id="1a705-131">id</span></span>|<span data-ttu-id="1a705-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a705-132">String</span></span>|<span data-ttu-id="1a705-133">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="1a705-133">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="1a705-134">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="1a705-134">appleIdentifier</span></span>|<span data-ttu-id="1a705-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a705-135">String</span></span>|<span data-ttu-id="1a705-136">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="1a705-136">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="1a705-137">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="1a705-137">topicIdentifier</span></span>|<span data-ttu-id="1a705-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a705-138">String</span></span>|<span data-ttu-id="1a705-139">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="1a705-139">Topic Id.</span></span>|
|<span data-ttu-id="1a705-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a705-140">lastModifiedDateTime</span></span>|<span data-ttu-id="1a705-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a705-141">DateTimeOffset</span></span>|<span data-ttu-id="1a705-142">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="1a705-142">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="1a705-143">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1a705-143">expirationDateTime</span></span>|<span data-ttu-id="1a705-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a705-144">DateTimeOffset</span></span>|<span data-ttu-id="1a705-145">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="1a705-145">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="1a705-146">certificado</span><span class="sxs-lookup"><span data-stu-id="1a705-146">certificate</span></span>|<span data-ttu-id="1a705-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a705-147">String</span></span>|<span data-ttu-id="1a705-148">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1a705-148">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1a705-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a705-149">Response</span></span>
<span data-ttu-id="1a705-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a705-150">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a705-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a705-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="1a705-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a705-152">Request</span></span>
<span data-ttu-id="1a705-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a705-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1a705-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a705-154">Response</span></span>
<span data-ttu-id="1a705-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a705-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



