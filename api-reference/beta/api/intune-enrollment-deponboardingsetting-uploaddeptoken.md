---
title: ação de uploadDepToken
description: Carrega um novo token do programa de inscrição do dispositivo
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e146ebe7d25c428c3451830eb7fa223096fff8af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886580"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="b4813-103">ação de uploadDepToken</span><span class="sxs-lookup"><span data-stu-id="b4813-103">uploadDepToken action</span></span>

> <span data-ttu-id="b4813-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b4813-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4813-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b4813-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4813-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b4813-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4813-107">Carrega um novo token do programa de inscrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b4813-107">Uploads a new Device Enrollment Program token</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4813-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4813-108">Prerequisites</span></span>
<span data-ttu-id="b4813-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4813-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4813-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4813-111">Permission type</span></span>|<span data-ttu-id="b4813-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4813-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4813-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4813-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4813-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4813-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b4813-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4813-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4813-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4813-116">Not supported.</span></span>|
|<span data-ttu-id="b4813-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4813-117">Application</span></span>|<span data-ttu-id="b4813-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4813-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4813-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4813-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="b4813-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4813-120">Request headers</span></span>
|<span data-ttu-id="b4813-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4813-121">Header</span></span>|<span data-ttu-id="b4813-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b4813-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4813-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4813-123">Authorization</span></span>|<span data-ttu-id="b4813-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4813-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4813-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b4813-125">Accept</span></span>|<span data-ttu-id="b4813-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4813-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4813-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4813-127">Request body</span></span>
<span data-ttu-id="b4813-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b4813-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b4813-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b4813-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b4813-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4813-130">Property</span></span>|<span data-ttu-id="b4813-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4813-131">Type</span></span>|<span data-ttu-id="b4813-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4813-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4813-133">appleId</span><span class="sxs-lookup"><span data-stu-id="b4813-133">appleId</span></span>|<span data-ttu-id="b4813-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4813-134">String</span></span>|<span data-ttu-id="b4813-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b4813-135">Not yet documented</span></span>|
|<span data-ttu-id="b4813-136">depToken</span><span class="sxs-lookup"><span data-stu-id="b4813-136">depToken</span></span>|<span data-ttu-id="b4813-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4813-137">String</span></span>|<span data-ttu-id="b4813-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b4813-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b4813-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4813-139">Response</span></span>
<span data-ttu-id="b4813-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b4813-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4813-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4813-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4813-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4813-142">Request</span></span>
<span data-ttu-id="b4813-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4813-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="b4813-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4813-144">Response</span></span>
<span data-ttu-id="b4813-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4813-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





