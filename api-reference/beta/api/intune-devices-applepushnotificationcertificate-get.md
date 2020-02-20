---
title: Obter applePushNotificationCertificate
description: Ler propriedades e relações do objeto applePushNotificationCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d778ac8f19864fac47c69ff81aacf8df2f0039e6
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162257"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="5c3bf-103">Obter applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="5c3bf-103">Get applePushNotificationCertificate</span></span>

> <span data-ttu-id="5c3bf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5c3bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c3bf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c3bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c3bf-106">Ler propriedades e relações do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="5c3bf-106">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c3bf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c3bf-107">Prerequisites</span></span>
<span data-ttu-id="5c3bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c3bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c3bf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c3bf-110">Permission type</span></span>|<span data-ttu-id="5c3bf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c3bf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c3bf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c3bf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c3bf-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c3bf-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5c3bf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c3bf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c3bf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c3bf-115">Not supported.</span></span>|
|<span data-ttu-id="5c3bf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c3bf-116">Application</span></span>|<span data-ttu-id="5c3bf-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c3bf-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c3bf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c3bf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c3bf-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5c3bf-119">Optional query parameters</span></span>
<span data-ttu-id="5c3bf-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5c3bf-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c3bf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c3bf-121">Request headers</span></span>
|<span data-ttu-id="5c3bf-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c3bf-122">Header</span></span>|<span data-ttu-id="5c3bf-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5c3bf-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c3bf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c3bf-124">Authorization</span></span>|<span data-ttu-id="5c3bf-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c3bf-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c3bf-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5c3bf-126">Accept</span></span>|<span data-ttu-id="5c3bf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5c3bf-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c3bf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c3bf-128">Request body</span></span>
<span data-ttu-id="5c3bf-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c3bf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c3bf-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c3bf-130">Response</span></span>
<span data-ttu-id="5c3bf-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c3bf-131">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c3bf-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c3bf-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c3bf-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c3bf-133">Request</span></span>
<span data-ttu-id="5c3bf-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c3bf-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="5c3bf-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c3bf-135">Response</span></span>
<span data-ttu-id="5c3bf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c3bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





