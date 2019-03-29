---
title: Função downloadApplePushNotificationCertificateSigningRequest
description: Baixa a solicitação de assinatura de certificado de notificação por push da Apple
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 09bbadd2e0874bdc461f965ff12544716e4de9d2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970195"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="a4dd0-103">Função downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="a4dd0-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="a4dd0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a4dd0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4dd0-105">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="a4dd0-105">Download Apple push notification certificate signing request</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4dd0-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a4dd0-106">Prerequisites</span></span>
<span data-ttu-id="a4dd0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4dd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4dd0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4dd0-109">Permission type</span></span>|<span data-ttu-id="a4dd0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a4dd0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4dd0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4dd0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4dd0-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4dd0-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a4dd0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4dd0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4dd0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4dd0-114">Not supported.</span></span>|
|<span data-ttu-id="a4dd0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4dd0-115">Application</span></span>|<span data-ttu-id="a4dd0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4dd0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4dd0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4dd0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="a4dd0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4dd0-118">Request headers</span></span>
|<span data-ttu-id="a4dd0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a4dd0-119">Header</span></span>|<span data-ttu-id="a4dd0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a4dd0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4dd0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4dd0-121">Authorization</span></span>|<span data-ttu-id="a4dd0-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4dd0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4dd0-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a4dd0-123">Accept</span></span>|<span data-ttu-id="a4dd0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a4dd0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4dd0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4dd0-125">Request body</span></span>
<span data-ttu-id="a4dd0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a4dd0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4dd0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4dd0-127">Response</span></span>
<span data-ttu-id="a4dd0-128">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4dd0-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4dd0-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4dd0-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4dd0-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4dd0-130">Request</span></span>
<span data-ttu-id="a4dd0-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4dd0-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="a4dd0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4dd0-132">Response</span></span>
<span data-ttu-id="a4dd0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a4dd0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```



