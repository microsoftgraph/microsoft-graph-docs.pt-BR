---
title: Excluir windowsPhone81CustomConfiguration
description: Exclui windowsPhone81CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b63de776d01eeb79f3b0bddde7189633bc3b5b15
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874260"
---
# <a name="delete-windowsphone81customconfiguration"></a><span data-ttu-id="c2c28-103">Excluir windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="c2c28-103">Delete windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="c2c28-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c2c28-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2c28-105">Exclui [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2c28-105">Deletes a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2c28-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c2c28-106">Prerequisites</span></span>
<span data-ttu-id="c2c28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2c28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2c28-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2c28-109">Permission type</span></span>|<span data-ttu-id="c2c28-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c2c28-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2c28-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2c28-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c2c28-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2c28-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c2c28-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2c28-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2c28-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2c28-114">Not supported.</span></span>|
|<span data-ttu-id="c2c28-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2c28-115">Application</span></span>|<span data-ttu-id="c2c28-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2c28-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2c28-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2c28-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c2c28-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2c28-118">Request headers</span></span>
|<span data-ttu-id="c2c28-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c2c28-119">Header</span></span>|<span data-ttu-id="c2c28-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c2c28-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2c28-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2c28-121">Authorization</span></span>|<span data-ttu-id="c2c28-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2c28-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2c28-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c2c28-123">Accept</span></span>|<span data-ttu-id="c2c28-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c2c28-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2c28-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2c28-125">Request body</span></span>
<span data-ttu-id="c2c28-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2c28-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2c28-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2c28-127">Response</span></span>
<span data-ttu-id="c2c28-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c2c28-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c2c28-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2c28-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2c28-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2c28-130">Request</span></span>
<span data-ttu-id="c2c28-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2c28-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c2c28-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2c28-132">Response</span></span>
<span data-ttu-id="c2c28-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2c28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



