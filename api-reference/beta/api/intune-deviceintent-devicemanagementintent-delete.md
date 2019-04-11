---
title: Excluir deviceManagementIntent
description: Exclui deviceManagementIntent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a50ae66cda65c8424a0b1497783c868eca0c5577
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783892"
---
# <a name="delete-devicemanagementintent"></a><span data-ttu-id="537ed-103">Excluir deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="537ed-103">Delete deviceManagementIntent</span></span>

> <span data-ttu-id="537ed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="537ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="537ed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="537ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="537ed-106">Exclui [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md).</span><span class="sxs-lookup"><span data-stu-id="537ed-106">Deletes a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="537ed-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="537ed-107">Prerequisites</span></span>
<span data-ttu-id="537ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="537ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="537ed-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="537ed-110">Permission type</span></span>|<span data-ttu-id="537ed-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="537ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="537ed-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="537ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="537ed-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="537ed-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="537ed-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="537ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="537ed-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="537ed-115">Not supported.</span></span>|
|<span data-ttu-id="537ed-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="537ed-116">Application</span></span>|<span data-ttu-id="537ed-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="537ed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="537ed-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="537ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/intents/{deviceManagementIntentId}
```

## <a name="request-headers"></a><span data-ttu-id="537ed-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="537ed-119">Request headers</span></span>
|<span data-ttu-id="537ed-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="537ed-120">Header</span></span>|<span data-ttu-id="537ed-121">Valor</span><span class="sxs-lookup"><span data-stu-id="537ed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="537ed-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="537ed-122">Authorization</span></span>|<span data-ttu-id="537ed-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="537ed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="537ed-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="537ed-124">Accept</span></span>|<span data-ttu-id="537ed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="537ed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="537ed-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="537ed-126">Request body</span></span>
<span data-ttu-id="537ed-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="537ed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="537ed-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="537ed-128">Response</span></span>
<span data-ttu-id="537ed-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="537ed-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="537ed-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="537ed-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="537ed-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="537ed-131">Request</span></span>
<span data-ttu-id="537ed-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="537ed-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}
```

### <a name="response"></a><span data-ttu-id="537ed-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="537ed-133">Response</span></span>
<span data-ttu-id="537ed-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="537ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





