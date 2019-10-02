---
title: Função downloadApplePushNotificationCertificateSigningRequest
description: Baixa a solicitação de assinatura de certificado de notificação por push da Apple
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3792a24a8c9868ab8b26e5493725f5929b888a2d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364631"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="f5b3d-103">Função downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="f5b3d-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="f5b3d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f5b3d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5b3d-105">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="f5b3d-105">Download Apple push notification certificate signing request</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5b3d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5b3d-106">Prerequisites</span></span>
<span data-ttu-id="f5b3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5b3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5b3d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5b3d-109">Permission type</span></span>|<span data-ttu-id="f5b3d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f5b3d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5b3d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5b3d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f5b3d-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5b3d-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f5b3d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5b3d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5b3d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5b3d-114">Not supported.</span></span>|
|<span data-ttu-id="f5b3d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5b3d-115">Application</span></span>|<span data-ttu-id="f5b3d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5b3d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5b3d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5b3d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="f5b3d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5b3d-118">Request headers</span></span>
|<span data-ttu-id="f5b3d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5b3d-119">Header</span></span>|<span data-ttu-id="f5b3d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f5b3d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5b3d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5b3d-121">Authorization</span></span>|<span data-ttu-id="f5b3d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5b3d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5b3d-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5b3d-123">Accept</span></span>|<span data-ttu-id="f5b3d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f5b3d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5b3d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5b3d-125">Request body</span></span>
<span data-ttu-id="f5b3d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5b3d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5b3d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5b3d-127">Response</span></span>
<span data-ttu-id="f5b3d-128">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5b3d-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5b3d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5b3d-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5b3d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5b3d-130">Request</span></span>
<span data-ttu-id="f5b3d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5b3d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="f5b3d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5b3d-132">Response</span></span>
<span data-ttu-id="f5b3d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5b3d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```




