---
title: Ação sendTestMessage
description: Envia mensagens de teste usando o notificationMessageTemplate especificado no local padrão
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 885f7c54baf4fbcbff98f2bfddbd05a372a09ccd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30249953"
---
# <a name="sendtestmessage-action"></a><span data-ttu-id="0c4e0-103">Ação sendTestMessage</span><span class="sxs-lookup"><span data-stu-id="0c4e0-103">sendTestMessage action</span></span>

> <span data-ttu-id="0c4e0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c4e0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c4e0-105">Envia mensagens de teste usando o notificationMessageTemplate especificado no local padrão</span><span class="sxs-lookup"><span data-stu-id="0c4e0-105">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c4e0-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c4e0-106">Prerequisites</span></span>
<span data-ttu-id="0c4e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0c4e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0c4e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c4e0-109">Permission type</span></span>|<span data-ttu-id="0c4e0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c4e0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c4e0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c4e0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0c4e0-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c4e0-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0c4e0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c4e0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c4e0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c4e0-114">Not supported.</span></span>|
|<span data-ttu-id="0c4e0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c4e0-115">Application</span></span>|<span data-ttu-id="0c4e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c4e0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c4e0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c4e0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

## <a name="request-headers"></a><span data-ttu-id="0c4e0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c4e0-118">Request headers</span></span>
|<span data-ttu-id="0c4e0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c4e0-119">Header</span></span>|<span data-ttu-id="0c4e0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0c4e0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c4e0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c4e0-121">Authorization</span></span>|<span data-ttu-id="0c4e0-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c4e0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c4e0-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c4e0-123">Accept</span></span>|<span data-ttu-id="0c4e0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0c4e0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c4e0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c4e0-125">Request body</span></span>
<span data-ttu-id="0c4e0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0c4e0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c4e0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c4e0-127">Response</span></span>
<span data-ttu-id="0c4e0-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0c4e0-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0c4e0-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c4e0-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c4e0-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c4e0-130">Request</span></span>
<span data-ttu-id="0c4e0-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c4e0-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

### <a name="response"></a><span data-ttu-id="0c4e0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c4e0-132">Response</span></span>
<span data-ttu-id="0c4e0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c4e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



