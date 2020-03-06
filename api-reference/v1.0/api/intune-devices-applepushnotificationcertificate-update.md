---
title: Atualizar applePushNotificationCertificate
description: Atualizar as propriedades de um objeto applePushNotificationCertificate.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7673193118fa1ec1aa7e82e94cfdd08d33911efa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513641"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="e4aaf-103">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="e4aaf-103">Update applePushNotificationCertificate</span></span>

<span data-ttu-id="e4aaf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4aaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4aaf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4aaf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4aaf-106">Atualizar as propriedades de um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="e4aaf-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4aaf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4aaf-107">Prerequisites</span></span>
<span data-ttu-id="e4aaf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4aaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4aaf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4aaf-110">Permission type</span></span>|<span data-ttu-id="e4aaf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4aaf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4aaf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4aaf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4aaf-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4aaf-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e4aaf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4aaf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4aaf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4aaf-115">Not supported.</span></span>|
|<span data-ttu-id="e4aaf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4aaf-116">Application</span></span>|<span data-ttu-id="e4aaf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4aaf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4aaf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4aaf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="e4aaf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4aaf-119">Request headers</span></span>
|<span data-ttu-id="e4aaf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4aaf-120">Header</span></span>|<span data-ttu-id="e4aaf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e4aaf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4aaf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4aaf-122">Authorization</span></span>|<span data-ttu-id="e4aaf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4aaf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4aaf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e4aaf-124">Accept</span></span>|<span data-ttu-id="e4aaf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4aaf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4aaf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4aaf-126">Request body</span></span>
<span data-ttu-id="e4aaf-127">No corpo da solicitação, forneça uma representação JSON do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="e4aaf-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="e4aaf-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="e4aaf-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="e4aaf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4aaf-129">Property</span></span>|<span data-ttu-id="e4aaf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4aaf-130">Type</span></span>|<span data-ttu-id="e4aaf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4aaf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4aaf-132">id</span><span class="sxs-lookup"><span data-stu-id="e4aaf-132">id</span></span>|<span data-ttu-id="e4aaf-133">String</span><span class="sxs-lookup"><span data-stu-id="e4aaf-133">String</span></span>|<span data-ttu-id="e4aaf-134">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="e4aaf-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="e4aaf-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="e4aaf-135">appleIdentifier</span></span>|<span data-ttu-id="e4aaf-136">String</span><span class="sxs-lookup"><span data-stu-id="e4aaf-136">String</span></span>|<span data-ttu-id="e4aaf-137">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="e4aaf-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="e4aaf-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="e4aaf-138">topicIdentifier</span></span>|<span data-ttu-id="e4aaf-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4aaf-139">String</span></span>|<span data-ttu-id="e4aaf-140">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="e4aaf-140">Topic Id.</span></span>|
|<span data-ttu-id="e4aaf-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4aaf-141">lastModifiedDateTime</span></span>|<span data-ttu-id="e4aaf-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4aaf-142">DateTimeOffset</span></span>|<span data-ttu-id="e4aaf-143">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="e4aaf-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="e4aaf-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e4aaf-144">expirationDateTime</span></span>|<span data-ttu-id="e4aaf-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4aaf-145">DateTimeOffset</span></span>|<span data-ttu-id="e4aaf-146">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="e4aaf-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="e4aaf-147">certificado</span><span class="sxs-lookup"><span data-stu-id="e4aaf-147">certificate</span></span>|<span data-ttu-id="e4aaf-148">String</span><span class="sxs-lookup"><span data-stu-id="e4aaf-148">String</span></span>|<span data-ttu-id="e4aaf-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e4aaf-149">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e4aaf-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4aaf-150">Response</span></span>
<span data-ttu-id="e4aaf-151">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4aaf-151">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4aaf-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4aaf-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4aaf-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4aaf-153">Request</span></span>
<span data-ttu-id="e4aaf-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4aaf-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e4aaf-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4aaf-155">Response</span></span>
<span data-ttu-id="e4aaf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4aaf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




