---
title: Obter applePushNotificationCertificate
description: Ler propriedades e relações do objeto applePushNotificationCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a96b66b155b1ffb7ffc158dd4ff25a711f1c1d93
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047606"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="40344-103">Obter applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="40344-103">Get applePushNotificationCertificate</span></span>

<span data-ttu-id="40344-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40344-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40344-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40344-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40344-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40344-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40344-107">Ler propriedades e relações do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="40344-107">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40344-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40344-108">Prerequisites</span></span>
<span data-ttu-id="40344-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40344-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40344-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40344-111">Permission type</span></span>|<span data-ttu-id="40344-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="40344-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40344-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40344-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40344-114">DeviceManagementServiceConfig. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="40344-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="40344-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40344-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40344-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40344-116">Not supported.</span></span>|
|<span data-ttu-id="40344-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40344-117">Application</span></span>|<span data-ttu-id="40344-118">DeviceManagementServiceConfig. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="40344-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40344-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40344-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40344-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="40344-120">Optional query parameters</span></span>
<span data-ttu-id="40344-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="40344-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40344-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40344-122">Request headers</span></span>
|<span data-ttu-id="40344-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40344-123">Header</span></span>|<span data-ttu-id="40344-124">Valor</span><span class="sxs-lookup"><span data-stu-id="40344-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40344-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="40344-125">Authorization</span></span>|<span data-ttu-id="40344-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40344-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40344-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40344-127">Accept</span></span>|<span data-ttu-id="40344-128">application/json</span><span class="sxs-lookup"><span data-stu-id="40344-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40344-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40344-129">Request body</span></span>
<span data-ttu-id="40344-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40344-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40344-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="40344-131">Response</span></span>
<span data-ttu-id="40344-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40344-132">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40344-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40344-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="40344-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40344-134">Request</span></span>
<span data-ttu-id="40344-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40344-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="40344-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="40344-136">Response</span></span>
<span data-ttu-id="40344-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40344-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 633

{
  "value": {
    "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
    "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
    "appleIdentifier": "Apple Identifier value",
    "topicIdentifier": "Topic Identifier value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificateUploadStatus": "Certificate Upload Status value",
    "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
    "certificateSerialNumber": "Certificate Serial Number value",
    "certificate": "Certificate value"
  }
}
```






