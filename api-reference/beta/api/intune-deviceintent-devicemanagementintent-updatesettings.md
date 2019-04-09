---
title: ação updateSettings
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a24d66d13c739ce12abd6e05dd75db9950244ef2
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522864"
---
# <a name="updatesettings-action"></a><span data-ttu-id="fb998-103">ação updateSettings</span><span class="sxs-lookup"><span data-stu-id="fb998-103">updateSettings action</span></span>

> <span data-ttu-id="fb998-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fb998-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb998-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb998-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb998-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fb998-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb998-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb998-107">Prerequisites</span></span>
<span data-ttu-id="fb998-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb998-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb998-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb998-110">Permission type</span></span>|<span data-ttu-id="fb998-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb998-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb998-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb998-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fb998-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb998-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb998-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb998-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb998-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb998-115">Not supported.</span></span>|
|<span data-ttu-id="fb998-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb998-116">Application</span></span>|<span data-ttu-id="fb998-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb998-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb998-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb998-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/updateSettings
```

## <a name="request-headers"></a><span data-ttu-id="fb998-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb998-119">Request headers</span></span>
|<span data-ttu-id="fb998-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb998-120">Header</span></span>|<span data-ttu-id="fb998-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fb998-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb998-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb998-122">Authorization</span></span>|<span data-ttu-id="fb998-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb998-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb998-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb998-124">Accept</span></span>|<span data-ttu-id="fb998-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb998-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb998-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb998-126">Request body</span></span>
<span data-ttu-id="fb998-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="fb998-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fb998-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="fb998-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fb998-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb998-129">Property</span></span>|<span data-ttu-id="fb998-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb998-130">Type</span></span>|<span data-ttu-id="fb998-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb998-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb998-132">settings</span><span class="sxs-lookup"><span data-stu-id="fb998-132">settings</span></span>|<span data-ttu-id="fb998-133">coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="fb998-133">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="fb998-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fb998-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fb998-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb998-135">Response</span></span>
<span data-ttu-id="fb998-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fb998-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fb998-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb998-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb998-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb998-138">Request</span></span>
<span data-ttu-id="fb998-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb998-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/updateSettings

Content-type: application/json
Content-length: 252

{
  "settings": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
      "id": "d68168e1-68e1-d681-e168-81d6e16881d6",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="fb998-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb998-140">Response</span></span>
<span data-ttu-id="fb998-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb998-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







