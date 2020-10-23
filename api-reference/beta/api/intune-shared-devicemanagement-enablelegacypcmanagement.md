---
title: ação enableLegacyPcManagement
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e0afd196dd8b0549d256d5401463f9007516ecbc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692839"
---
# <a name="enablelegacypcmanagement-action"></a><span data-ttu-id="5b98c-103">ação enableLegacyPcManagement</span><span class="sxs-lookup"><span data-stu-id="5b98c-103">enableLegacyPcManagement action</span></span>

<span data-ttu-id="5b98c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b98c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b98c-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5b98c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5b98c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5b98c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b98c-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b98c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b98c-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5b98c-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b98c-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5b98c-109">Prerequisites</span></span>
<span data-ttu-id="5b98c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b98c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b98c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b98c-112">Permission type</span></span>|<span data-ttu-id="5b98c-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5b98c-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b98c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b98c-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5b98c-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="5b98c-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5b98c-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b98c-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b98c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b98c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b98c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b98c-118">Not supported.</span></span>|
|<span data-ttu-id="5b98c-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b98c-119">Application</span></span>||
| <span data-ttu-id="5b98c-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="5b98c-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5b98c-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b98c-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b98c-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b98c-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableLegacyPcManagement
```

## <a name="request-headers"></a><span data-ttu-id="5b98c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b98c-123">Request headers</span></span>
|<span data-ttu-id="5b98c-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b98c-124">Header</span></span>|<span data-ttu-id="5b98c-125">Valor</span><span class="sxs-lookup"><span data-stu-id="5b98c-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b98c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b98c-126">Authorization</span></span>|<span data-ttu-id="5b98c-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b98c-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b98c-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5b98c-128">Accept</span></span>|<span data-ttu-id="5b98c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="5b98c-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b98c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b98c-130">Request body</span></span>
<span data-ttu-id="5b98c-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b98c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b98c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b98c-132">Response</span></span>
<span data-ttu-id="5b98c-133">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5b98c-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5b98c-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b98c-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b98c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b98c-135">Request</span></span>
<span data-ttu-id="5b98c-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b98c-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableLegacyPcManagement
```

### <a name="response"></a><span data-ttu-id="5b98c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b98c-137">Response</span></span>
<span data-ttu-id="5b98c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b98c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```













