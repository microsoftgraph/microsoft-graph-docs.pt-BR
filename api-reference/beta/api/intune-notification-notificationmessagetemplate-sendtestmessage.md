---
title: Ação sendTestMessage
description: Envia mensagens de teste usando o notificationMessageTemplate especificado no local padrão
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dbac678815c5f190fae53747dbf522eecbe20ed9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396984"
---
# <a name="sendtestmessage-action"></a><span data-ttu-id="df968-103">Ação sendTestMessage</span><span class="sxs-lookup"><span data-stu-id="df968-103">sendTestMessage action</span></span>

> <span data-ttu-id="df968-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="df968-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="df968-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="df968-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df968-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="df968-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df968-107">Envia mensagens de teste usando o notificationMessageTemplate especificado no local padrão</span><span class="sxs-lookup"><span data-stu-id="df968-107">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df968-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df968-108">Prerequisites</span></span>
<span data-ttu-id="df968-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="df968-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="df968-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df968-111">Permission type</span></span>|<span data-ttu-id="df968-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df968-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df968-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df968-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df968-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df968-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="df968-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df968-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df968-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df968-116">Not supported.</span></span>|
|<span data-ttu-id="df968-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df968-117">Application</span></span>|<span data-ttu-id="df968-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df968-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df968-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df968-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

## <a name="request-headers"></a><span data-ttu-id="df968-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df968-120">Request headers</span></span>
|<span data-ttu-id="df968-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df968-121">Header</span></span>|<span data-ttu-id="df968-122">Valor</span><span class="sxs-lookup"><span data-stu-id="df968-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df968-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="df968-123">Authorization</span></span>|<span data-ttu-id="df968-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df968-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df968-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df968-125">Accept</span></span>|<span data-ttu-id="df968-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df968-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df968-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df968-127">Request body</span></span>
<span data-ttu-id="df968-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df968-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df968-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="df968-129">Response</span></span>
<span data-ttu-id="df968-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="df968-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="df968-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df968-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="df968-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df968-132">Request</span></span>
<span data-ttu-id="df968-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df968-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

### <a name="response"></a><span data-ttu-id="df968-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="df968-134">Response</span></span>
<span data-ttu-id="df968-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df968-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




