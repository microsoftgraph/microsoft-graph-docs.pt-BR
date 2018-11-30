---
title: ação de enableLegacyPcManagement
description: Ainda não documentado
ms.openlocfilehash: c9feaaea9e8b3c9573db95b6dd3f9aaae91243e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040026"
---
# <a name="enablelegacypcmanagement-action"></a><span data-ttu-id="6c15b-103">ação de enableLegacyPcManagement</span><span class="sxs-lookup"><span data-stu-id="6c15b-103">enableLegacyPcManagement action</span></span>

> <span data-ttu-id="6c15b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6c15b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c15b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6c15b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c15b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6c15b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c15b-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6c15b-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6c15b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c15b-108">Prerequisites</span></span>
<span data-ttu-id="6c15b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c15b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c15b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c15b-111">Permission type</span></span>|<span data-ttu-id="6c15b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c15b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c15b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c15b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6c15b-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="6c15b-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6c15b-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c15b-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c15b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c15b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c15b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c15b-117">Not supported.</span></span>|
|<span data-ttu-id="6c15b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c15b-118">Application</span></span>|<span data-ttu-id="6c15b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c15b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c15b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c15b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableLegacyPcManagement
```

## <a name="request-headers"></a><span data-ttu-id="6c15b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c15b-121">Request headers</span></span>
|<span data-ttu-id="6c15b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c15b-122">Header</span></span>|<span data-ttu-id="6c15b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6c15b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c15b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c15b-124">Authorization</span></span>|<span data-ttu-id="6c15b-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c15b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c15b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="6c15b-126">Accept</span></span>|<span data-ttu-id="6c15b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6c15b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c15b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c15b-128">Request body</span></span>
<span data-ttu-id="6c15b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c15b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c15b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c15b-130">Response</span></span>
<span data-ttu-id="6c15b-131">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6c15b-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6c15b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c15b-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="6c15b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c15b-133">Request</span></span>
<span data-ttu-id="6c15b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c15b-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableLegacyPcManagement
```

### <a name="response"></a><span data-ttu-id="6c15b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c15b-135">Response</span></span>
<span data-ttu-id="6c15b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c15b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





