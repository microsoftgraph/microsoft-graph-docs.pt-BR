---
title: Ação createCopy
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f87ff93f982d01d02ef2fd20f1536aec78c3493e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128905"
---
# <a name="createcopy-action"></a><span data-ttu-id="2de5e-103">Ação createCopy</span><span class="sxs-lookup"><span data-stu-id="2de5e-103">createCopy action</span></span>

<span data-ttu-id="2de5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2de5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2de5e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2de5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2de5e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2de5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2de5e-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2de5e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2de5e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2de5e-108">Prerequisites</span></span>
<span data-ttu-id="2de5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2de5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2de5e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2de5e-111">Permission type</span></span>|<span data-ttu-id="2de5e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2de5e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2de5e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2de5e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2de5e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2de5e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2de5e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2de5e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2de5e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2de5e-116">Not supported.</span></span>|
|<span data-ttu-id="2de5e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2de5e-117">Application</span></span>|<span data-ttu-id="2de5e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2de5e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2de5e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2de5e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/createCopy
```

## <a name="request-headers"></a><span data-ttu-id="2de5e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2de5e-120">Request headers</span></span>
|<span data-ttu-id="2de5e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2de5e-121">Header</span></span>|<span data-ttu-id="2de5e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2de5e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2de5e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2de5e-123">Authorization</span></span>|<span data-ttu-id="2de5e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2de5e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2de5e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2de5e-125">Accept</span></span>|<span data-ttu-id="2de5e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2de5e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2de5e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2de5e-127">Request body</span></span>
<span data-ttu-id="2de5e-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="2de5e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2de5e-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="2de5e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2de5e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2de5e-130">Property</span></span>|<span data-ttu-id="2de5e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2de5e-131">Type</span></span>|<span data-ttu-id="2de5e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2de5e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2de5e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2de5e-133">displayName</span></span>|<span data-ttu-id="2de5e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2de5e-134">String</span></span>|<span data-ttu-id="2de5e-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2de5e-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2de5e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2de5e-136">Response</span></span>
<span data-ttu-id="2de5e-137">Se tiver êxito, essa ação retornará um código `200 OK` de resposta e um [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2de5e-137">If successful, this action returns a `200 OK` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2de5e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2de5e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2de5e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2de5e-139">Request</span></span>
<span data-ttu-id="2de5e-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2de5e-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/createCopy

Content-type: application/json
Content-length: 43

{
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="2de5e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2de5e-141">Response</span></span>
<span data-ttu-id="2de5e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2de5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 418

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntent",
    "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
    "displayName": "Display Name value",
    "description": "Description value",
    "isAssigned": true,
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "templateId": "Template Id value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




