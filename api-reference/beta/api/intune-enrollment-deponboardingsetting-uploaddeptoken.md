---
title: ação de uploadDepToken
description: Carrega um novo token do programa de inscrição do dispositivo
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 98c663b80ecfbc2fb1641b8db8bb48af9215c885
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417046"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="2d93b-103">ação de uploadDepToken</span><span class="sxs-lookup"><span data-stu-id="2d93b-103">uploadDepToken action</span></span>

> <span data-ttu-id="2d93b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2d93b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2d93b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2d93b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2d93b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2d93b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d93b-107">Carrega um novo token do programa de inscrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="2d93b-107">Uploads a new Device Enrollment Program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d93b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d93b-108">Prerequisites</span></span>
<span data-ttu-id="2d93b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2d93b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2d93b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d93b-111">Permission type</span></span>|<span data-ttu-id="2d93b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2d93b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d93b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d93b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2d93b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d93b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2d93b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d93b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d93b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d93b-116">Not supported.</span></span>|
|<span data-ttu-id="2d93b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d93b-117">Application</span></span>|<span data-ttu-id="2d93b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d93b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d93b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d93b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="2d93b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d93b-120">Request headers</span></span>
|<span data-ttu-id="2d93b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d93b-121">Header</span></span>|<span data-ttu-id="2d93b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2d93b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d93b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d93b-123">Authorization</span></span>|<span data-ttu-id="2d93b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d93b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d93b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2d93b-125">Accept</span></span>|<span data-ttu-id="2d93b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2d93b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d93b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d93b-127">Request body</span></span>
<span data-ttu-id="2d93b-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="2d93b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2d93b-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="2d93b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2d93b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d93b-130">Property</span></span>|<span data-ttu-id="2d93b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d93b-131">Type</span></span>|<span data-ttu-id="2d93b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d93b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d93b-133">appleId</span><span class="sxs-lookup"><span data-stu-id="2d93b-133">appleId</span></span>|<span data-ttu-id="2d93b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d93b-134">String</span></span>|<span data-ttu-id="2d93b-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2d93b-135">Not yet documented</span></span>|
|<span data-ttu-id="2d93b-136">depToken</span><span class="sxs-lookup"><span data-stu-id="2d93b-136">depToken</span></span>|<span data-ttu-id="2d93b-137">String</span><span class="sxs-lookup"><span data-stu-id="2d93b-137">String</span></span>|<span data-ttu-id="2d93b-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2d93b-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2d93b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d93b-139">Response</span></span>
<span data-ttu-id="2d93b-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2d93b-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2d93b-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d93b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d93b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d93b-142">Request</span></span>
<span data-ttu-id="2d93b-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d93b-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="2d93b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d93b-144">Response</span></span>
<span data-ttu-id="2d93b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d93b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




