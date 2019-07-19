---
title: Função downloadApplePushNotificationCertificateSigningRequest
description: Baixa a solicitação de assinatura de certificado de notificação por push da Apple
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ddd3de89b4374cf3e222c76fa68eb37a5c8cf57f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959394"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="a4643-103">Função downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="a4643-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="a4643-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a4643-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4643-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a4643-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4643-106">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="a4643-106">Download Apple push notification certificate signing request</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4643-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a4643-107">Prerequisites</span></span>
<span data-ttu-id="a4643-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4643-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4643-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4643-110">Permission type</span></span>|<span data-ttu-id="a4643-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a4643-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4643-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4643-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4643-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4643-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a4643-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4643-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4643-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4643-115">Not supported.</span></span>|
|<span data-ttu-id="a4643-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4643-116">Application</span></span>|<span data-ttu-id="a4643-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4643-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4643-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4643-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="a4643-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4643-119">Request headers</span></span>
|<span data-ttu-id="a4643-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a4643-120">Header</span></span>|<span data-ttu-id="a4643-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a4643-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4643-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4643-122">Authorization</span></span>|<span data-ttu-id="a4643-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4643-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4643-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a4643-124">Accept</span></span>|<span data-ttu-id="a4643-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4643-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4643-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4643-126">Request body</span></span>
<span data-ttu-id="a4643-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a4643-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4643-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4643-128">Response</span></span>
<span data-ttu-id="a4643-129">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4643-129">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4643-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4643-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4643-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4643-131">Request</span></span>
<span data-ttu-id="a4643-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4643-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="a4643-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4643-133">Response</span></span>
<span data-ttu-id="a4643-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a4643-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```





