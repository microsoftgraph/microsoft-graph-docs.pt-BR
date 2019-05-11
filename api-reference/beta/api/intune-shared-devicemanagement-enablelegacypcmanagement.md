---
title: ação enableLegacyPcManagement
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d6be39db71c6fa6d1105db65b05c071627f08d5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898772"
---
# <a name="enablelegacypcmanagement-action"></a><span data-ttu-id="2518d-103">ação enableLegacyPcManagement</span><span class="sxs-lookup"><span data-stu-id="2518d-103">enableLegacyPcManagement action</span></span>

> <span data-ttu-id="2518d-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2518d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2518d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2518d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2518d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2518d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2518d-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2518d-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2518d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2518d-108">Prerequisites</span></span>
<span data-ttu-id="2518d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2518d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2518d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2518d-111">Permission type</span></span>|<span data-ttu-id="2518d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2518d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2518d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2518d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2518d-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="2518d-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2518d-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2518d-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2518d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2518d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2518d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2518d-117">Not supported.</span></span>|
|<span data-ttu-id="2518d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2518d-118">Application</span></span>|<span data-ttu-id="2518d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2518d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2518d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2518d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableLegacyPcManagement
```

## <a name="request-headers"></a><span data-ttu-id="2518d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2518d-121">Request headers</span></span>
|<span data-ttu-id="2518d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2518d-122">Header</span></span>|<span data-ttu-id="2518d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2518d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2518d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2518d-124">Authorization</span></span>|<span data-ttu-id="2518d-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2518d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2518d-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2518d-126">Accept</span></span>|<span data-ttu-id="2518d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2518d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2518d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2518d-128">Request body</span></span>
<span data-ttu-id="2518d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2518d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2518d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2518d-130">Response</span></span>
<span data-ttu-id="2518d-131">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2518d-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2518d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2518d-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="2518d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2518d-133">Request</span></span>
<span data-ttu-id="2518d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2518d-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableLegacyPcManagement
```

### <a name="response"></a><span data-ttu-id="2518d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2518d-135">Response</span></span>
<span data-ttu-id="2518d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2518d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





