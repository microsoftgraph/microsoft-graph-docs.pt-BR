---
title: Excluir deviceConfigurationUserStatus
description: Exclui deviceConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b28d56fa80b58d70dcbff7121a8d674d6be7c73b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918851"
---
# <a name="delete-deviceconfigurationuserstatus"></a><span data-ttu-id="93ffa-103">Excluir deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="93ffa-103">Delete deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="93ffa-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="93ffa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93ffa-105">Exclui [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="93ffa-105">Deletes a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="93ffa-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="93ffa-106">Prerequisites</span></span>
<span data-ttu-id="93ffa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93ffa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93ffa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93ffa-109">Permission type</span></span>|<span data-ttu-id="93ffa-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="93ffa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93ffa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93ffa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="93ffa-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93ffa-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="93ffa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93ffa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93ffa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93ffa-114">Not supported.</span></span>|
|<span data-ttu-id="93ffa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93ffa-115">Application</span></span>|<span data-ttu-id="93ffa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93ffa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93ffa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93ffa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="93ffa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93ffa-118">Request headers</span></span>
|<span data-ttu-id="93ffa-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93ffa-119">Header</span></span>|<span data-ttu-id="93ffa-120">Valor</span><span class="sxs-lookup"><span data-stu-id="93ffa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93ffa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="93ffa-121">Authorization</span></span>|<span data-ttu-id="93ffa-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93ffa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93ffa-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="93ffa-123">Accept</span></span>|<span data-ttu-id="93ffa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="93ffa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93ffa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93ffa-125">Request body</span></span>
<span data-ttu-id="93ffa-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93ffa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93ffa-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="93ffa-127">Response</span></span>
<span data-ttu-id="93ffa-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="93ffa-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="93ffa-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93ffa-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="93ffa-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93ffa-130">Request</span></span>
<span data-ttu-id="93ffa-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93ffa-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="93ffa-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="93ffa-132">Response</span></span>
<span data-ttu-id="93ffa-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93ffa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



