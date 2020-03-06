---
title: Excluir localizedNotificationMessage
description: Exclui localizedNotificationMessage.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c46b84d631693809fb38863b5684d1085dfbade
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512780"
---
# <a name="delete-localizednotificationmessage"></a><span data-ttu-id="34fde-103">Excluir localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="34fde-103">Delete localizedNotificationMessage</span></span>

<span data-ttu-id="34fde-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34fde-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34fde-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34fde-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34fde-106">Exclui [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="34fde-106">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34fde-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34fde-107">Prerequisites</span></span>
<span data-ttu-id="34fde-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34fde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34fde-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34fde-110">Permission type</span></span>|<span data-ttu-id="34fde-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34fde-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34fde-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34fde-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34fde-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34fde-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="34fde-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34fde-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34fde-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34fde-115">Not supported.</span></span>|
|<span data-ttu-id="34fde-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34fde-116">Application</span></span>|<span data-ttu-id="34fde-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34fde-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34fde-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34fde-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="34fde-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34fde-119">Request headers</span></span>
|<span data-ttu-id="34fde-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34fde-120">Header</span></span>|<span data-ttu-id="34fde-121">Valor</span><span class="sxs-lookup"><span data-stu-id="34fde-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34fde-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="34fde-122">Authorization</span></span>|<span data-ttu-id="34fde-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34fde-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34fde-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="34fde-124">Accept</span></span>|<span data-ttu-id="34fde-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34fde-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34fde-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34fde-126">Request body</span></span>
<span data-ttu-id="34fde-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34fde-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34fde-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="34fde-128">Response</span></span>
<span data-ttu-id="34fde-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="34fde-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="34fde-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34fde-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="34fde-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34fde-131">Request</span></span>
<span data-ttu-id="34fde-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34fde-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="34fde-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="34fde-133">Response</span></span>
<span data-ttu-id="34fde-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34fde-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




