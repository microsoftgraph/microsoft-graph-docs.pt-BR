---
title: Atualizar applePushNotificationCertificate
description: Atualizar as propriedades de um objeto applePushNotificationCertificate.
author: tfitzmac
ms.openlocfilehash: b81a6a9dc887ddfea387a904219bba529729d01a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335340"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="2f71a-103">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="2f71a-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="2f71a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2f71a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f71a-105">Atualizar as propriedades de um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="2f71a-105">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f71a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f71a-106">Prerequisites</span></span>
<span data-ttu-id="2f71a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f71a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f71a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f71a-109">Permission type</span></span>|<span data-ttu-id="2f71a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f71a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f71a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f71a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f71a-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f71a-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2f71a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f71a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f71a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f71a-114">Not supported.</span></span>|
|<span data-ttu-id="2f71a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f71a-115">Application</span></span>|<span data-ttu-id="2f71a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f71a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f71a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f71a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="2f71a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f71a-118">Request headers</span></span>
|<span data-ttu-id="2f71a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f71a-119">Header</span></span>|<span data-ttu-id="2f71a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2f71a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f71a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f71a-121">Authorization</span></span>|<span data-ttu-id="2f71a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f71a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f71a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2f71a-123">Accept</span></span>|<span data-ttu-id="2f71a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2f71a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f71a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f71a-125">Request body</span></span>
<span data-ttu-id="2f71a-126">No corpo da solicitação, forneça uma representação JSON do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="2f71a-126">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="2f71a-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="2f71a-127">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="2f71a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f71a-128">Property</span></span>|<span data-ttu-id="2f71a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f71a-129">Type</span></span>|<span data-ttu-id="2f71a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f71a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f71a-131">id</span><span class="sxs-lookup"><span data-stu-id="2f71a-131">id</span></span>|<span data-ttu-id="2f71a-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f71a-132">String</span></span>|<span data-ttu-id="2f71a-133">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="2f71a-133">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="2f71a-134">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="2f71a-134">appleIdentifier</span></span>|<span data-ttu-id="2f71a-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f71a-135">String</span></span>|<span data-ttu-id="2f71a-136">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="2f71a-136">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="2f71a-137">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="2f71a-137">topicIdentifier</span></span>|<span data-ttu-id="2f71a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f71a-138">String</span></span>|<span data-ttu-id="2f71a-139">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="2f71a-139">Topic Id.</span></span>|
|<span data-ttu-id="2f71a-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f71a-140">lastModifiedDateTime</span></span>|<span data-ttu-id="2f71a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f71a-141">DateTimeOffset</span></span>|<span data-ttu-id="2f71a-142">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="2f71a-142">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="2f71a-143">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2f71a-143">expirationDateTime</span></span>|<span data-ttu-id="2f71a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f71a-144">DateTimeOffset</span></span>|<span data-ttu-id="2f71a-145">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="2f71a-145">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="2f71a-146">certificado</span><span class="sxs-lookup"><span data-stu-id="2f71a-146">certificate</span></span>|<span data-ttu-id="2f71a-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f71a-147">String</span></span>|<span data-ttu-id="2f71a-148">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2f71a-148">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2f71a-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f71a-149">Response</span></span>
<span data-ttu-id="2f71a-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f71a-150">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f71a-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f71a-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f71a-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f71a-152">Request</span></span>
<span data-ttu-id="2f71a-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f71a-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f71a-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f71a-154">Response</span></span>
<span data-ttu-id="2f71a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f71a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



