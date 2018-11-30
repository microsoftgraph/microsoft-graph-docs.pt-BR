---
title: Excluir windowsUpdateForBusinessConfiguration
description: Exclui windowsUpdateForBusinessConfiguration.
ms.openlocfilehash: b0a69a29f8262da976fc19e814332e294960ec60
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003795"
---
# <a name="delete-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="9f7b6-103">Excluir windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="9f7b6-103">Delete windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="9f7b6-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9f7b6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f7b6-105">Exclui [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f7b6-105">Deletes a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f7b6-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9f7b6-106">Prerequisites</span></span>
<span data-ttu-id="9f7b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f7b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f7b6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f7b6-109">Permission type</span></span>|<span data-ttu-id="9f7b6-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9f7b6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f7b6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f7b6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f7b6-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f7b6-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f7b6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f7b6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f7b6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f7b6-114">Not supported.</span></span>|
|<span data-ttu-id="9f7b6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f7b6-115">Application</span></span>|<span data-ttu-id="9f7b6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f7b6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f7b6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f7b6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9f7b6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f7b6-118">Request headers</span></span>
|<span data-ttu-id="9f7b6-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9f7b6-119">Header</span></span>|<span data-ttu-id="9f7b6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9f7b6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f7b6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f7b6-121">Authorization</span></span>|<span data-ttu-id="9f7b6-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f7b6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f7b6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9f7b6-123">Accept</span></span>|<span data-ttu-id="9f7b6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9f7b6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f7b6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f7b6-125">Request body</span></span>
<span data-ttu-id="9f7b6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9f7b6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f7b6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f7b6-127">Response</span></span>
<span data-ttu-id="9f7b6-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9f7b6-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9f7b6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f7b6-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f7b6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f7b6-130">Request</span></span>
<span data-ttu-id="9f7b6-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f7b6-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9f7b6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f7b6-132">Response</span></span>
<span data-ttu-id="9f7b6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f7b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



