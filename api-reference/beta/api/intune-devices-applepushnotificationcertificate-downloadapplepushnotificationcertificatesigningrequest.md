---
title: Função downloadApplePushNotificationCertificateSigningRequest
description: Baixa a solicitação de assinatura de certificado de notificação por push da Apple
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 72f58d8941bbe19b278490fb92cc471f17afa5aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414687"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="42d8b-103">Função downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="42d8b-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="42d8b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="42d8b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="42d8b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="42d8b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42d8b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="42d8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42d8b-107">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="42d8b-107">Download Apple push notification certificate signing request</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42d8b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42d8b-108">Prerequisites</span></span>
<span data-ttu-id="42d8b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="42d8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="42d8b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42d8b-111">Permission type</span></span>|<span data-ttu-id="42d8b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42d8b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42d8b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42d8b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42d8b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42d8b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="42d8b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42d8b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42d8b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42d8b-116">Not supported.</span></span>|
|<span data-ttu-id="42d8b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42d8b-117">Application</span></span>|<span data-ttu-id="42d8b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42d8b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42d8b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42d8b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="42d8b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42d8b-120">Request headers</span></span>
|<span data-ttu-id="42d8b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42d8b-121">Header</span></span>|<span data-ttu-id="42d8b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="42d8b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42d8b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="42d8b-123">Authorization</span></span>|<span data-ttu-id="42d8b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42d8b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42d8b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42d8b-125">Accept</span></span>|<span data-ttu-id="42d8b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42d8b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42d8b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42d8b-127">Request body</span></span>
<span data-ttu-id="42d8b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42d8b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42d8b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="42d8b-129">Response</span></span>
<span data-ttu-id="42d8b-130">Se tiver êxito, esta função retornará um código de resposta `200 OK` e uma Cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42d8b-130">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42d8b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42d8b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="42d8b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42d8b-132">Request</span></span>
<span data-ttu-id="42d8b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42d8b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="42d8b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="42d8b-134">Response</span></span>
<span data-ttu-id="42d8b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42d8b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```




