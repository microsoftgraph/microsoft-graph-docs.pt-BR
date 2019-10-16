---
title: Ação syncMicrosoftStoreForBusinessApps
description: Sincroniza a conta do Intune com o Microsoft Store For Business
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 39ee98b3eba5cafed655cab168f6f419709597aa
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537117"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="7cfff-103">Ação syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="7cfff-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="7cfff-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7cfff-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7cfff-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7cfff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7cfff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7cfff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cfff-107">Sincroniza a conta do Intune com o Microsoft Store For Business</span><span class="sxs-lookup"><span data-stu-id="7cfff-107">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7cfff-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7cfff-108">Prerequisites</span></span>
<span data-ttu-id="7cfff-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cfff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cfff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cfff-111">Permission type</span></span>|<span data-ttu-id="7cfff-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7cfff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cfff-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cfff-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7cfff-114">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="7cfff-114">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="7cfff-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cfff-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7cfff-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cfff-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cfff-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cfff-117">Not supported.</span></span>|
|<span data-ttu-id="7cfff-118">Application</span><span class="sxs-lookup"><span data-stu-id="7cfff-118">Application</span></span>||
| <span data-ttu-id="7cfff-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="7cfff-119">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="7cfff-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cfff-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cfff-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cfff-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="7cfff-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cfff-122">Request headers</span></span>
|<span data-ttu-id="7cfff-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7cfff-123">Header</span></span>|<span data-ttu-id="7cfff-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7cfff-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cfff-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cfff-125">Authorization</span></span>|<span data-ttu-id="7cfff-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cfff-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cfff-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7cfff-127">Accept</span></span>|<span data-ttu-id="7cfff-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7cfff-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cfff-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7cfff-129">Request body</span></span>
<span data-ttu-id="7cfff-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7cfff-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cfff-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cfff-131">Response</span></span>
<span data-ttu-id="7cfff-132">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7cfff-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7cfff-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7cfff-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="7cfff-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cfff-134">Request</span></span>
<span data-ttu-id="7cfff-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7cfff-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="7cfff-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cfff-136">Response</span></span>
<span data-ttu-id="7cfff-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7cfff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









