---
title: ação enableLegacyPcManagement
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 469c1c661d2ad6fec98a5225becde26124942cd1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390298"
---
# <a name="enablelegacypcmanagement-action"></a><span data-ttu-id="0b574-103">ação enableLegacyPcManagement</span><span class="sxs-lookup"><span data-stu-id="0b574-103">enableLegacyPcManagement action</span></span>

<span data-ttu-id="0b574-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b574-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b574-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0b574-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0b574-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0b574-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b574-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b574-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b574-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0b574-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0b574-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b574-109">Prerequisites</span></span>
<span data-ttu-id="0b574-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b574-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b574-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b574-112">Permission type</span></span>|<span data-ttu-id="0b574-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b574-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b574-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b574-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0b574-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0b574-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="0b574-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b574-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b574-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b574-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b574-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b574-118">Not supported.</span></span>|
|<span data-ttu-id="0b574-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b574-119">Application</span></span>||
| <span data-ttu-id="0b574-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0b574-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="0b574-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b574-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b574-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b574-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableLegacyPcManagement
```

## <a name="request-headers"></a><span data-ttu-id="0b574-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b574-123">Request headers</span></span>
|<span data-ttu-id="0b574-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b574-124">Header</span></span>|<span data-ttu-id="0b574-125">Valor</span><span class="sxs-lookup"><span data-stu-id="0b574-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b574-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b574-126">Authorization</span></span>|<span data-ttu-id="0b574-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b574-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b574-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b574-128">Accept</span></span>|<span data-ttu-id="0b574-129">application/json</span><span class="sxs-lookup"><span data-stu-id="0b574-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b574-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b574-130">Request body</span></span>
<span data-ttu-id="0b574-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0b574-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b574-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b574-132">Response</span></span>
<span data-ttu-id="0b574-133">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0b574-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0b574-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b574-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="0b574-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b574-135">Request</span></span>
<span data-ttu-id="0b574-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b574-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableLegacyPcManagement
```

### <a name="response"></a><span data-ttu-id="0b574-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b574-137">Response</span></span>
<span data-ttu-id="0b574-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b574-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```











