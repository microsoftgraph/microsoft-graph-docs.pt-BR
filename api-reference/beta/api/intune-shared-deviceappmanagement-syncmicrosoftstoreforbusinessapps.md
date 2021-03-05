---
title: Ação syncMicrosoftStoreForBusinessApps
description: Sincroniza a conta do Intune com o Microsoft Store For Business
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f1be868185e634ba74f9f58f1ab4c388efcf5ed3
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474866"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="92b76-103">Ação syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="92b76-103">syncMicrosoftStoreForBusinessApps action</span></span>

<span data-ttu-id="92b76-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92b76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92b76-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="92b76-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="92b76-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="92b76-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92b76-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92b76-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92b76-108">Sincroniza a conta do Intune com o Microsoft Store For Business</span><span class="sxs-lookup"><span data-stu-id="92b76-108">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="92b76-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92b76-109">Prerequisites</span></span>
<span data-ttu-id="92b76-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92b76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92b76-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92b76-112">Permission type</span></span>|<span data-ttu-id="92b76-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92b76-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92b76-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92b76-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="92b76-115">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="92b76-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="92b76-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92b76-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="92b76-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92b76-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92b76-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92b76-118">Not supported.</span></span>|
|<span data-ttu-id="92b76-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92b76-119">Application</span></span>||
| <span data-ttu-id="92b76-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="92b76-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="92b76-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92b76-121">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92b76-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92b76-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="92b76-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92b76-123">Request headers</span></span>
|<span data-ttu-id="92b76-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92b76-124">Header</span></span>|<span data-ttu-id="92b76-125">Valor</span><span class="sxs-lookup"><span data-stu-id="92b76-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92b76-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="92b76-126">Authorization</span></span>|<span data-ttu-id="92b76-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92b76-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92b76-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92b76-128">Accept</span></span>|<span data-ttu-id="92b76-129">application/json</span><span class="sxs-lookup"><span data-stu-id="92b76-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92b76-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92b76-130">Request body</span></span>
<span data-ttu-id="92b76-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92b76-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92b76-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="92b76-132">Response</span></span>
<span data-ttu-id="92b76-133">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="92b76-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="92b76-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92b76-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="92b76-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92b76-135">Request</span></span>
<span data-ttu-id="92b76-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92b76-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="92b76-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="92b76-137">Response</span></span>
<span data-ttu-id="92b76-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92b76-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```










