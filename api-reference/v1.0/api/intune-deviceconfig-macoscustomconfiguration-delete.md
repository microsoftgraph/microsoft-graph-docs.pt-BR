---
title: Excluir macOSCustomConfiguration
description: Exclui macOSCustomConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9257047a8fc4f8ffa0a5955896a176ce46e965ef
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366045"
---
# <a name="delete-macoscustomconfiguration"></a><span data-ttu-id="5da24-103">Excluir macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="5da24-103">Delete macOSCustomConfiguration</span></span>

> <span data-ttu-id="5da24-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5da24-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5da24-105">Exclui [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5da24-105">Deletes a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5da24-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5da24-106">Prerequisites</span></span>
<span data-ttu-id="5da24-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5da24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5da24-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5da24-109">Permission type</span></span>|<span data-ttu-id="5da24-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5da24-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5da24-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5da24-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5da24-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5da24-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5da24-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5da24-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5da24-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5da24-114">Not supported.</span></span>|
|<span data-ttu-id="5da24-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5da24-115">Application</span></span>|<span data-ttu-id="5da24-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5da24-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5da24-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5da24-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5da24-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5da24-118">Request headers</span></span>
|<span data-ttu-id="5da24-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5da24-119">Header</span></span>|<span data-ttu-id="5da24-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5da24-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5da24-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5da24-121">Authorization</span></span>|<span data-ttu-id="5da24-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5da24-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5da24-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5da24-123">Accept</span></span>|<span data-ttu-id="5da24-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5da24-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5da24-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5da24-125">Request body</span></span>
<span data-ttu-id="5da24-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5da24-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5da24-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5da24-127">Response</span></span>
<span data-ttu-id="5da24-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5da24-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5da24-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5da24-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="5da24-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5da24-130">Request</span></span>
<span data-ttu-id="5da24-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5da24-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5da24-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5da24-132">Response</span></span>
<span data-ttu-id="5da24-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5da24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




