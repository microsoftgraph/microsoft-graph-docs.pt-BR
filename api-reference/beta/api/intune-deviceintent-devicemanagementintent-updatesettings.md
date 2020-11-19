---
title: ação updateSettings
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b9b4536cfb6e255bfb45377b89d30c0a7ff592d7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49229748"
---
# <a name="updatesettings-action"></a><span data-ttu-id="d75bc-103">ação updateSettings</span><span class="sxs-lookup"><span data-stu-id="d75bc-103">updateSettings action</span></span>

<span data-ttu-id="d75bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d75bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d75bc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d75bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d75bc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d75bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d75bc-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d75bc-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d75bc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d75bc-108">Prerequisites</span></span>
<span data-ttu-id="d75bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d75bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d75bc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d75bc-111">Permission type</span></span>|<span data-ttu-id="d75bc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d75bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d75bc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d75bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d75bc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d75bc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d75bc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d75bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d75bc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d75bc-116">Not supported.</span></span>|
|<span data-ttu-id="d75bc-117">Application</span><span class="sxs-lookup"><span data-stu-id="d75bc-117">Application</span></span>|<span data-ttu-id="d75bc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d75bc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d75bc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d75bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/updateSettings
```

## <a name="request-headers"></a><span data-ttu-id="d75bc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d75bc-120">Request headers</span></span>
|<span data-ttu-id="d75bc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d75bc-121">Header</span></span>|<span data-ttu-id="d75bc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d75bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d75bc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d75bc-123">Authorization</span></span>|<span data-ttu-id="d75bc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d75bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d75bc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d75bc-125">Accept</span></span>|<span data-ttu-id="d75bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d75bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d75bc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d75bc-127">Request body</span></span>
<span data-ttu-id="d75bc-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d75bc-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d75bc-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d75bc-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d75bc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d75bc-130">Property</span></span>|<span data-ttu-id="d75bc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d75bc-131">Type</span></span>|<span data-ttu-id="d75bc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d75bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d75bc-133">settings</span><span class="sxs-lookup"><span data-stu-id="d75bc-133">settings</span></span>|<span data-ttu-id="d75bc-134">coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d75bc-134">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="d75bc-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d75bc-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d75bc-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d75bc-136">Response</span></span>
<span data-ttu-id="d75bc-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d75bc-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d75bc-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d75bc-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d75bc-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d75bc-139">Request</span></span>
<span data-ttu-id="d75bc-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d75bc-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d75bc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d75bc-141">Response</span></span>
<span data-ttu-id="d75bc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d75bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




