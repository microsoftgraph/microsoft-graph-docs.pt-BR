---
title: ação updateSettings
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 089777a99bbf1e433e24af41fe3674b005575a1c
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37185942"
---
# <a name="updatesettings-action"></a><span data-ttu-id="c857e-103">ação updateSettings</span><span class="sxs-lookup"><span data-stu-id="c857e-103">updateSettings action</span></span>

> <span data-ttu-id="c857e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c857e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c857e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c857e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c857e-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c857e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c857e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c857e-107">Prerequisites</span></span>
<span data-ttu-id="c857e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c857e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c857e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c857e-110">Permission type</span></span>|<span data-ttu-id="c857e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c857e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c857e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c857e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c857e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c857e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c857e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c857e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c857e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c857e-115">Not supported.</span></span>|
|<span data-ttu-id="c857e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c857e-116">Application</span></span>|<span data-ttu-id="c857e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c857e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c857e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c857e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/updateSettings
```

## <a name="request-headers"></a><span data-ttu-id="c857e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c857e-119">Request headers</span></span>
|<span data-ttu-id="c857e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c857e-120">Header</span></span>|<span data-ttu-id="c857e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c857e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c857e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c857e-122">Authorization</span></span>|<span data-ttu-id="c857e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c857e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c857e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c857e-124">Accept</span></span>|<span data-ttu-id="c857e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c857e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c857e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c857e-126">Request body</span></span>
<span data-ttu-id="c857e-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c857e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c857e-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="c857e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c857e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c857e-129">Property</span></span>|<span data-ttu-id="c857e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c857e-130">Type</span></span>|<span data-ttu-id="c857e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c857e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c857e-132">settings</span><span class="sxs-lookup"><span data-stu-id="c857e-132">settings</span></span>|<span data-ttu-id="c857e-133">coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="c857e-133">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="c857e-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c857e-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c857e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c857e-135">Response</span></span>
<span data-ttu-id="c857e-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c857e-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c857e-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c857e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c857e-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c857e-138">Request</span></span>
<span data-ttu-id="c857e-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c857e-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c857e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c857e-140">Response</span></span>
<span data-ttu-id="c857e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c857e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




