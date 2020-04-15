---
title: Atualizar applePushNotificationCertificate
description: Atualizar as propriedades de um objeto applePushNotificationCertificate.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 34254267440a80701f27583a64df6dfae608655e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456824"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="264ac-103">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="264ac-103">Update applePushNotificationCertificate</span></span>

<span data-ttu-id="264ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="264ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="264ac-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="264ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="264ac-106">Atualizar as propriedades de um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="264ac-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="264ac-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="264ac-107">Prerequisites</span></span>
<span data-ttu-id="264ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="264ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="264ac-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="264ac-110">Permission type</span></span>|<span data-ttu-id="264ac-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="264ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="264ac-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="264ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="264ac-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="264ac-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="264ac-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="264ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="264ac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="264ac-115">Not supported.</span></span>|
|<span data-ttu-id="264ac-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="264ac-116">Application</span></span>|<span data-ttu-id="264ac-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="264ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="264ac-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="264ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="264ac-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="264ac-119">Request headers</span></span>
|<span data-ttu-id="264ac-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="264ac-120">Header</span></span>|<span data-ttu-id="264ac-121">Valor</span><span class="sxs-lookup"><span data-stu-id="264ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="264ac-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="264ac-122">Authorization</span></span>|<span data-ttu-id="264ac-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="264ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="264ac-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="264ac-124">Accept</span></span>|<span data-ttu-id="264ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="264ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="264ac-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="264ac-126">Request body</span></span>
<span data-ttu-id="264ac-127">No corpo da solicitação, forneça uma representação JSON do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="264ac-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="264ac-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="264ac-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="264ac-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="264ac-129">Property</span></span>|<span data-ttu-id="264ac-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="264ac-130">Type</span></span>|<span data-ttu-id="264ac-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="264ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="264ac-132">id</span><span class="sxs-lookup"><span data-stu-id="264ac-132">id</span></span>|<span data-ttu-id="264ac-133">String</span><span class="sxs-lookup"><span data-stu-id="264ac-133">String</span></span>|<span data-ttu-id="264ac-134">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="264ac-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="264ac-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="264ac-135">appleIdentifier</span></span>|<span data-ttu-id="264ac-136">String</span><span class="sxs-lookup"><span data-stu-id="264ac-136">String</span></span>|<span data-ttu-id="264ac-137">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="264ac-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="264ac-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="264ac-138">topicIdentifier</span></span>|<span data-ttu-id="264ac-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="264ac-139">String</span></span>|<span data-ttu-id="264ac-140">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="264ac-140">Topic Id.</span></span>|
|<span data-ttu-id="264ac-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="264ac-141">lastModifiedDateTime</span></span>|<span data-ttu-id="264ac-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="264ac-142">DateTimeOffset</span></span>|<span data-ttu-id="264ac-143">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="264ac-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="264ac-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="264ac-144">expirationDateTime</span></span>|<span data-ttu-id="264ac-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="264ac-145">DateTimeOffset</span></span>|<span data-ttu-id="264ac-146">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="264ac-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="264ac-147">certificado</span><span class="sxs-lookup"><span data-stu-id="264ac-147">certificate</span></span>|<span data-ttu-id="264ac-148">String</span><span class="sxs-lookup"><span data-stu-id="264ac-148">String</span></span>|<span data-ttu-id="264ac-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="264ac-149">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="264ac-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="264ac-150">Response</span></span>
<span data-ttu-id="264ac-151">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="264ac-151">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="264ac-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="264ac-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="264ac-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="264ac-153">Request</span></span>
<span data-ttu-id="264ac-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="264ac-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="264ac-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="264ac-155">Response</span></span>
<span data-ttu-id="264ac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="264ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






