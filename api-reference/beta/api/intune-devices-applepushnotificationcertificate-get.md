---
title: Obter applePushNotificationCertificate
description: Ler propriedades e relações do objeto applePushNotificationCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 95373eb1ef3cbf5bd6b382a2302464c15af7f198
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136521"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="c4f57-103">Obter applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="c4f57-103">Get applePushNotificationCertificate</span></span>

<span data-ttu-id="c4f57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4f57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4f57-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4f57-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4f57-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4f57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4f57-107">Ler propriedades e relações do objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="c4f57-107">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4f57-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4f57-108">Prerequisites</span></span>
<span data-ttu-id="c4f57-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4f57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4f57-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4f57-111">Permission type</span></span>|<span data-ttu-id="c4f57-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4f57-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4f57-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4f57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4f57-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4f57-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c4f57-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4f57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4f57-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4f57-116">Not supported.</span></span>|
|<span data-ttu-id="c4f57-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4f57-117">Application</span></span>|<span data-ttu-id="c4f57-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4f57-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4f57-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4f57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4f57-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c4f57-120">Optional query parameters</span></span>
<span data-ttu-id="c4f57-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c4f57-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4f57-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4f57-122">Request headers</span></span>
|<span data-ttu-id="c4f57-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4f57-123">Header</span></span>|<span data-ttu-id="c4f57-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c4f57-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4f57-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4f57-125">Authorization</span></span>|<span data-ttu-id="c4f57-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4f57-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4f57-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4f57-127">Accept</span></span>|<span data-ttu-id="c4f57-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c4f57-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4f57-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4f57-129">Request body</span></span>
<span data-ttu-id="c4f57-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4f57-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4f57-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4f57-131">Response</span></span>
<span data-ttu-id="c4f57-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4f57-132">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4f57-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4f57-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4f57-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4f57-134">Request</span></span>
<span data-ttu-id="c4f57-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4f57-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="c4f57-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4f57-136">Response</span></span>
<span data-ttu-id="c4f57-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4f57-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




