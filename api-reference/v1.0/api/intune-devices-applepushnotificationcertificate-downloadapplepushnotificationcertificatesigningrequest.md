---
title: Função downloadApplePushNotificationCertificateSigningRequest
description: Baixa a solicitação de assinatura de certificado de notificação por push da Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88542997e432220d23102b6b2d02372f43ac909a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756159"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="4f3a6-103">Função downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="4f3a6-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

<span data-ttu-id="4f3a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f3a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f3a6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f3a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f3a6-106">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="4f3a6-106">Download Apple push notification certificate signing request</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f3a6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f3a6-107">Prerequisites</span></span>
<span data-ttu-id="4f3a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f3a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f3a6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f3a6-110">Permission type</span></span>|<span data-ttu-id="4f3a6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f3a6-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f3a6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f3a6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f3a6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f3a6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4f3a6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f3a6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f3a6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f3a6-115">Not supported.</span></span>|
|<span data-ttu-id="4f3a6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f3a6-116">Application</span></span>|<span data-ttu-id="4f3a6-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f3a6-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f3a6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f3a6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="4f3a6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f3a6-119">Request headers</span></span>
|<span data-ttu-id="4f3a6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f3a6-120">Header</span></span>|<span data-ttu-id="4f3a6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4f3a6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f3a6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f3a6-122">Authorization</span></span>|<span data-ttu-id="4f3a6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f3a6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f3a6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f3a6-124">Accept</span></span>|<span data-ttu-id="4f3a6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f3a6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f3a6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f3a6-126">Request body</span></span>
<span data-ttu-id="4f3a6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f3a6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f3a6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f3a6-128">Response</span></span>
<span data-ttu-id="4f3a6-129">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f3a6-129">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f3a6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f3a6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f3a6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f3a6-131">Request</span></span>
<span data-ttu-id="4f3a6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f3a6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="4f3a6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f3a6-133">Response</span></span>
<span data-ttu-id="4f3a6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f3a6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```




