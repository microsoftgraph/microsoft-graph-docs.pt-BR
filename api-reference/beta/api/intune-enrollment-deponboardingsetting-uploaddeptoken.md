---
title: Ação uploadDepToken
description: Carrega um novo token do programa de registro de dispositivos
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c1366b774299e7c23e2185d54c610478ec2727eb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466868"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="ac0b9-103">Ação uploadDepToken</span><span class="sxs-lookup"><span data-stu-id="ac0b9-103">uploadDepToken action</span></span>

<span data-ttu-id="ac0b9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ac0b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac0b9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ac0b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac0b9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ac0b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac0b9-107">Carrega um novo token do programa de registro de dispositivos</span><span class="sxs-lookup"><span data-stu-id="ac0b9-107">Uploads a new Device Enrollment Program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac0b9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ac0b9-108">Prerequisites</span></span>
<span data-ttu-id="ac0b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac0b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac0b9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac0b9-111">Permission type</span></span>|<span data-ttu-id="ac0b9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ac0b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac0b9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac0b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac0b9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac0b9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ac0b9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac0b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac0b9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac0b9-116">Not supported.</span></span>|
|<span data-ttu-id="ac0b9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac0b9-117">Application</span></span>|<span data-ttu-id="ac0b9-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac0b9-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac0b9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac0b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="ac0b9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac0b9-120">Request headers</span></span>
|<span data-ttu-id="ac0b9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac0b9-121">Header</span></span>|<span data-ttu-id="ac0b9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ac0b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac0b9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac0b9-123">Authorization</span></span>|<span data-ttu-id="ac0b9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac0b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac0b9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ac0b9-125">Accept</span></span>|<span data-ttu-id="ac0b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac0b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac0b9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac0b9-127">Request body</span></span>
<span data-ttu-id="ac0b9-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ac0b9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ac0b9-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ac0b9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ac0b9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac0b9-130">Property</span></span>|<span data-ttu-id="ac0b9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac0b9-131">Type</span></span>|<span data-ttu-id="ac0b9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac0b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac0b9-133">appleId</span><span class="sxs-lookup"><span data-stu-id="ac0b9-133">appleId</span></span>|<span data-ttu-id="ac0b9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac0b9-134">String</span></span>|<span data-ttu-id="ac0b9-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ac0b9-135">Not yet documented</span></span>|
|<span data-ttu-id="ac0b9-136">depToken</span><span class="sxs-lookup"><span data-stu-id="ac0b9-136">depToken</span></span>|<span data-ttu-id="ac0b9-137">String</span><span class="sxs-lookup"><span data-stu-id="ac0b9-137">String</span></span>|<span data-ttu-id="ac0b9-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ac0b9-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ac0b9-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac0b9-139">Response</span></span>
<span data-ttu-id="ac0b9-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ac0b9-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ac0b9-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac0b9-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac0b9-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac0b9-142">Request</span></span>
<span data-ttu-id="ac0b9-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac0b9-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="ac0b9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac0b9-144">Response</span></span>
<span data-ttu-id="ac0b9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac0b9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





