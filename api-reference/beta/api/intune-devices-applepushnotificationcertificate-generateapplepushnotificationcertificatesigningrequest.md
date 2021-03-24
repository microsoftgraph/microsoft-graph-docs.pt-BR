---
title: ação generateApplePushNotificationCertificateSigningRequest
description: Baixa a solicitação de assinatura de certificado de notificação por push da Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d72aa518df5ce437a99b2dca9a46c7c0bcc0dfb0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136528"
---
# <a name="generateapplepushnotificationcertificatesigningrequest-action"></a><span data-ttu-id="8e845-103">ação generateApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="8e845-103">generateApplePushNotificationCertificateSigningRequest action</span></span>

<span data-ttu-id="8e845-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e845-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e845-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e845-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e845-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e845-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e845-107">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="8e845-107">Download Apple push notification certificate signing request</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e845-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e845-108">Prerequisites</span></span>
<span data-ttu-id="8e845-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e845-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e845-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e845-111">Permission type</span></span>|<span data-ttu-id="8e845-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e845-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e845-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e845-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e845-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e845-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8e845-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e845-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e845-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e845-116">Not supported.</span></span>|
|<span data-ttu-id="8e845-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e845-117">Application</span></span>|<span data-ttu-id="8e845-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e845-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e845-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e845-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/applePushNotificationCertificate/generateApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="8e845-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e845-120">Request headers</span></span>
|<span data-ttu-id="8e845-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e845-121">Header</span></span>|<span data-ttu-id="8e845-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8e845-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e845-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e845-123">Authorization</span></span>|<span data-ttu-id="8e845-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e845-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e845-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e845-125">Accept</span></span>|<span data-ttu-id="8e845-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e845-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e845-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e845-127">Request body</span></span>
<span data-ttu-id="8e845-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e845-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e845-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e845-129">Response</span></span>
<span data-ttu-id="8e845-130">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e845-130">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e845-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e845-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e845-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e845-132">Request</span></span>
<span data-ttu-id="8e845-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e845-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate/generateApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="8e845-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e845-134">Response</span></span>
<span data-ttu-id="8e845-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e845-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Generate Apple Push Notification Certificate Signing Request value"
}
```




