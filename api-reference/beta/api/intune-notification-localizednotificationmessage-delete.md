---
title: Excluir localizedNotificationMessage
description: Exclui localizedNotificationMessage.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 300e87165afe3e68efa0fdf8aaaa307d9aa2c5fb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34957882"
---
# <a name="delete-localizednotificationmessage"></a><span data-ttu-id="bd450-103">Excluir localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="bd450-103">Delete localizedNotificationMessage</span></span>

> <span data-ttu-id="bd450-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bd450-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd450-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bd450-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd450-106">Exclui [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="bd450-106">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd450-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bd450-107">Prerequisites</span></span>
<span data-ttu-id="bd450-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd450-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd450-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd450-110">Permission type</span></span>|<span data-ttu-id="bd450-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bd450-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd450-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd450-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bd450-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd450-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bd450-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd450-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd450-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd450-115">Not supported.</span></span>|
|<span data-ttu-id="bd450-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd450-116">Application</span></span>|<span data-ttu-id="bd450-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd450-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd450-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd450-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="bd450-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd450-119">Request headers</span></span>
|<span data-ttu-id="bd450-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bd450-120">Header</span></span>|<span data-ttu-id="bd450-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bd450-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd450-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd450-122">Authorization</span></span>|<span data-ttu-id="bd450-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd450-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd450-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bd450-124">Accept</span></span>|<span data-ttu-id="bd450-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bd450-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd450-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd450-126">Request body</span></span>
<span data-ttu-id="bd450-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd450-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd450-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd450-128">Response</span></span>
<span data-ttu-id="bd450-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bd450-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bd450-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd450-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd450-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd450-131">Request</span></span>
<span data-ttu-id="bd450-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd450-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="bd450-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd450-133">Response</span></span>
<span data-ttu-id="bd450-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd450-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





