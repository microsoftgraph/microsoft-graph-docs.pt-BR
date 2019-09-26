---
title: ação enableLegacyPcManagement
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d10ff8ae4f6727c6741eecb3f37099a82f7abf63
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194646"
---
# <a name="enablelegacypcmanagement-action"></a><span data-ttu-id="30673-103">ação enableLegacyPcManagement</span><span class="sxs-lookup"><span data-stu-id="30673-103">enableLegacyPcManagement action</span></span>

> <span data-ttu-id="30673-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="30673-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="30673-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="30673-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30673-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30673-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30673-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="30673-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="30673-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30673-108">Prerequisites</span></span>
<span data-ttu-id="30673-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30673-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30673-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30673-111">Permission type</span></span>|<span data-ttu-id="30673-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30673-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30673-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30673-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="30673-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="30673-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="30673-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30673-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="30673-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30673-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30673-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30673-117">Not supported.</span></span>|
|<span data-ttu-id="30673-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30673-118">Application</span></span>||
| <span data-ttu-id="30673-119">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="30673-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="30673-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30673-120">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30673-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30673-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableLegacyPcManagement
```

## <a name="request-headers"></a><span data-ttu-id="30673-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30673-122">Request headers</span></span>
|<span data-ttu-id="30673-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30673-123">Header</span></span>|<span data-ttu-id="30673-124">Valor</span><span class="sxs-lookup"><span data-stu-id="30673-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30673-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="30673-125">Authorization</span></span>|<span data-ttu-id="30673-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30673-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30673-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30673-127">Accept</span></span>|<span data-ttu-id="30673-128">application/json</span><span class="sxs-lookup"><span data-stu-id="30673-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30673-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30673-129">Request body</span></span>
<span data-ttu-id="30673-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30673-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30673-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="30673-131">Response</span></span>
<span data-ttu-id="30673-132">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="30673-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="30673-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30673-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="30673-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30673-134">Request</span></span>
<span data-ttu-id="30673-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30673-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableLegacyPcManagement
```

### <a name="response"></a><span data-ttu-id="30673-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="30673-136">Response</span></span>
<span data-ttu-id="30673-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30673-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









