---
title: Ação sendTestMessage
description: Envia mensagens de teste usando o notificationMessageTemplate especificado no local padrão
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ea854f0bbad6647c82e50e8299d05ae7f3a68108
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054025"
---
# <a name="sendtestmessage-action"></a><span data-ttu-id="67bec-103">Ação sendTestMessage</span><span class="sxs-lookup"><span data-stu-id="67bec-103">sendTestMessage action</span></span>

<span data-ttu-id="67bec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67bec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67bec-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67bec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67bec-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67bec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67bec-107">Envia mensagens de teste usando o notificationMessageTemplate especificado no local padrão</span><span class="sxs-lookup"><span data-stu-id="67bec-107">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67bec-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67bec-108">Prerequisites</span></span>
<span data-ttu-id="67bec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67bec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67bec-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67bec-111">Permission type</span></span>|<span data-ttu-id="67bec-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67bec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67bec-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67bec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67bec-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67bec-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="67bec-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67bec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67bec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67bec-116">Not supported.</span></span>|
|<span data-ttu-id="67bec-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67bec-117">Application</span></span>|<span data-ttu-id="67bec-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67bec-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67bec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67bec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

## <a name="request-headers"></a><span data-ttu-id="67bec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67bec-120">Request headers</span></span>
|<span data-ttu-id="67bec-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67bec-121">Header</span></span>|<span data-ttu-id="67bec-122">Valor</span><span class="sxs-lookup"><span data-stu-id="67bec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67bec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="67bec-123">Authorization</span></span>|<span data-ttu-id="67bec-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67bec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67bec-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67bec-125">Accept</span></span>|<span data-ttu-id="67bec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67bec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67bec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67bec-127">Request body</span></span>
<span data-ttu-id="67bec-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67bec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67bec-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="67bec-129">Response</span></span>
<span data-ttu-id="67bec-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="67bec-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="67bec-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67bec-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="67bec-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67bec-132">Request</span></span>
<span data-ttu-id="67bec-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67bec-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

### <a name="response"></a><span data-ttu-id="67bec-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="67bec-134">Response</span></span>
<span data-ttu-id="67bec-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67bec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






