---
title: Função downloadApplePushNotificationCertificateSigningRequest
description: Baixa a solicitação de assinatura de certificado de notificação por push da Apple
author: tfitzmac
ms.openlocfilehash: 99a62c456dd8d4f0e0779c44b800169e5de57164
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315516"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="7ed3e-103">Função downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="7ed3e-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="7ed3e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7ed3e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ed3e-105">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="7ed3e-105">Download Apple push notification certificate signing request</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7ed3e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7ed3e-106">Prerequisites</span></span>
<span data-ttu-id="7ed3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ed3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ed3e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ed3e-109">Permission type</span></span>|<span data-ttu-id="7ed3e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7ed3e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ed3e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ed3e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7ed3e-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ed3e-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7ed3e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ed3e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ed3e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ed3e-114">Not supported.</span></span>|
|<span data-ttu-id="7ed3e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ed3e-115">Application</span></span>|<span data-ttu-id="7ed3e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ed3e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ed3e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ed3e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="7ed3e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed3e-118">Request headers</span></span>
|<span data-ttu-id="7ed3e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ed3e-119">Header</span></span>|<span data-ttu-id="7ed3e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7ed3e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ed3e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ed3e-121">Authorization</span></span>|<span data-ttu-id="7ed3e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ed3e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ed3e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7ed3e-123">Accept</span></span>|<span data-ttu-id="7ed3e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7ed3e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ed3e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed3e-125">Request body</span></span>
<span data-ttu-id="7ed3e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ed3e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ed3e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ed3e-127">Response</span></span>
<span data-ttu-id="7ed3e-128">Se tiver êxito, esta função retornará um código de resposta `200 OK` e uma Cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ed3e-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ed3e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ed3e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="7ed3e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed3e-130">Request</span></span>
<span data-ttu-id="7ed3e-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ed3e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="7ed3e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ed3e-132">Response</span></span>
<span data-ttu-id="7ed3e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ed3e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```



